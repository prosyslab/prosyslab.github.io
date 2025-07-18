---
title: "문제가 문제다(2): 높이 올라가야 멀리 보인다"
date: 2025-07-03
author: Kihong Heo
kor_author: 허기홍
tags:
  - 연구
  - 문제찾기
  - Optimuzz
classes: wide
---

_([이전 이야기]({{ site.url }}{{ site.baseurl }}/sky-and-star)에서 이어진다.)_

## 높이 올라가야 멀리 보인다: Optimuzz 이야기
한 가지 문제를 훌륭하게 풀다보면, 여러 좋은 문제들이 눈에 들어온다는 이야기이다.
당면한 문제를 풀 때는 제대로.
잘 되는 것만 쫓지 말고, 안되는 것은 왜 안되는지 확실히 알고 넘어가야 훗날 좋은 문제로 다시 찾아온다.
남들 뒤꽁무니를 따르는 것이 아니라 나만의 길을 제대로 걷고 있다면, 거기서 만나는 풍경도 세상에서 나만 아는 비밀.
거기에 숨겨진 문제는 이 길을 와보지 않은 남들은 발견 못할 신선한 것일 수 밖에.

2023년 한창 [TurboTV]({{ site.url }}{{ site.baseurl }}/turbotv/)를 만들던 때였다.
졸업한 승완이, 재성이, AWS의 이준영 박사와 함께 작업한 TurboFan의 [번역 검산기(translation validation)](https://github.com/prosyslab/pl-wiki/wiki/번역-검산(Translation-Validation))이다.
번역 검산기란 컴파일러의 최적화가 옳은지 논리적으로 검사하는 기술이다.
컴파일러 최적화는 사용자가 작성한 코드를 좀 더 빠르게 돌아가도록 여기 저기 바꾼다.
하지만 컴파일러에 오류가 있으면 이렇게 바꾸는 과정에서 원래 사람의 의도와 다른 프로그램이 만들어진다.
번역 검산기는 이렇게 바뀌기 전과 후 프로그램이 같은 동작을 하는지를 검사한다.
보통 컴파일러는 매우 크고 복잡한 소프트웨어이기 때문에 현장에서 번역검산기의 도움은 꼭 필요하고, 전세계에서 가장 널리
쓰이는 컴파일러인 LLVM의 개발과정에는 이미 통합되어 있다. (자세한 내용은 [여기](https://github.com/prosyslab/pl-wiki/wiki/TurboTV)에)

어느 정도 TurboTV가 완성이 되었다고 생각한 연구 막바지 일이었다.
성능을 평가하고 실제 TurboFan의 오류를 찾기 위해서 마구실행기(fuzzer)와 결합해보기로 했다.
번역검산기의 특성상 오류를 유발하는 입력 프로그램 (즉, 최적화 대상 프로그램) 있어야 해당 오류를 잡아낼 수 있기 때문이다.
TurboFan은 JavaScript 프로그램을 입력으로 받는 컴파일러이다.
JavaScript 프로그램을 자동으로 생성하여 오류를 찾는 기술은 학계에서 제법 오래 발전해 왔기 때문에 최신 기술을 가져다 사용하면 어렵지 않게 우리의 성과를 뽑낼 수 있을거라 생각했다.
마침 구글에서 만들어서 널리 쓰이고 있는 마구실행기가 공개되어 있었다. 아주 제격이라고 생각했다.

하지만 역시 처음엔 쉬워보이는 일도 들여다보면 문제투성이다.
컴파일러의 오류 지점을 이미 알고 있는 실험 상황이었지만, 마구실행기는 그 지점으로 향하는 프로그램을 만들어내지 못했다.
하루를 돌리고, 이틀을 돌려도 오류 근처도 가지 못했다.
컴파일러가 너무나 복잡하고 큰 프로그램인데다가 JavaScript 언어도 복잡해서 탐색 공간이 너무 넓은 것이 문제였다.
마구실행기는 순전히 무작위로 프로그램을 생성하니까 사막에서 바늘 찾는 것과 다를 바가 없었다.
이 연구의 초점은 마구실행기의 성능이 아니었기 때문에 일단은 이 문제를 묻어두기로 했다.
마구실행기를 우리 상황에 맞게 수동으로 튜닝하고 TurboTV의 성능을 평가하는 것으로 실험을 마무리 했다.

2023년 8월에 TurboTV 논문을 ICSE에 제출하고 나서 마구실행기와 번역검산기를 결합하는 문제를 골똘히 생각해 보았다.
제한된 실험 환경에서도 그 정도 탐색 능력이라면, 실제 현장에서 숨은 오류를 잘 찾아내지 못할게 분명했다.
살펴보니 번역 검산기가 현장에서 쓰이고 있기는 하지만 입력은 늘 사람이 만들어 주는 듯 했다.
개발자들이 직접 컴파일러를 수정하고, 변경한 지점을 거치는 입력을 손수 한 두개 만들어 주는게 현실이었다.
그러다보니 숨은 오류를 놓치는 경우도 많았다. 이걸 자동으로 해야하지 않을까?
효율적인 번역검산을 위해서 특정 최적화를 일으키는 프로그램을 마구 생산하는 기술이 필요하지 않을까?
이런 문제는 아무도 제대로 집중하고 있지 않은 듯 했다.
우리가 TurboTV를 만드는 길을 갔기에, 그 와중에 마구실행기와 번역검산기를 결합하는 선택을 했기에 가능했던 흔치 않은 시선이라고 본다.
또한 마침 프로그램의 특정 지점에 집중하는 입력을 만드는 비슷한 연구가 연구실에서 활발히 진행되고 있었다.
[지향성 퍼징]({{ site.url }}{{ site.baseurl }}/dafl-story),
[지향성 단위 테스트 생성기]({{ site.url }}{{site.baseurl}}/sky-and-star)에 이어
최적화 지향성 컴파일러 입력 생성기까지.
“지향성” 3부작이 완성되는 순간이었다.

우리만의 뚜렷한 시선을 갖추니 새로운 기회도 보였다.
우연히 페이스북에서 본 Amazon 연구상 공고였다.
Amazon 연구상은 정기적으로 몇 개 분야를 정해서 연구제안서를 공모하고 그 중 우수한 연구에 연구비를 지원하는 프로그램이다.
과거 몇 년간 우리 분야의 공모는 없어서 신경을 안쓰고 지냈던 차였다.
그런데 마침 그 해 뜬 자동 검증(automated reasoning) 분야의 공모가 내 눈길을 사로잡았다.
마침 기존 연구비도 다 떨어져가던 차라 새로운 제안서를 써야하기도 했고, 우리의 시선이 얼마나 제대로인지 외부에 확인해보고 싶기도 했다.
기쁜 마음으로 제안서를 써내려갔다.
“최적화 지향성 컴파일러 입력 생성기”를 중심으로 컴파일러 안전성을 효율적으로 검사하는 방법에 관해 밑그림을 그렸다.
TurboTV를 만들었던 학생들과 이준영 박사의 도움 덕분에 일필휘지였다.
그 해 겨울, ICSE에 제출했던 논문도 채택이 되었고, 다음 봄이 되자 예상대로 Amazon에서도 수상작으로 선정해주었다.
문제의 중요성을 모두 인정해 준 것이다.

그 때부터는 거침없는 항해였다.
TurboTV를 함께 만든 [재성](https://doitman.kr)이와 당시 학부 연구생으로 들어와 지금은 대학원생이된 [봉준](https://bongjunj.github.io)이가 앞장섰다.
번역검산과 컴파일러 전문가인 이준영 박사도 여전히 함께하여 큰 도움을 주었다.
재성이와 봉준이는 거리낌없이 치고나가면서 앞에 놓인 장애물을 매주 차근차근 부수기 시작했다.
그렇게 [Optimuzz](https://prosys.kaist.ac.kr/optimuzz/) 프로젝트가 시작되었다.
어느정도 시스템이 성숙하자 야생으로 나가보기로 했다.
세상에서 가장 널리 쓰이는 컴파일러인 LLVM에 우리 기술을 적용해 봤더니 오류가 무더기로 쏟아져 나왔다.
TurboFan에서도 기존보다 월등히 나은 성능을 보였다.
성공적인 기술임을 확신했다. 약 1년 정도 연구를 거쳐 2024년 11월, 결과를 PLDI에 제출했다.
역시나 다들 우리의 시선에 공감했다. 평가는 매우 긍정적이었고 무난하게 채택되었다. 특히, 아래와 같은 심사평이 뿌듯했다:
> It opens a new direction of compiler fuzzing, i.e., guided compiler fuzzing. (Reviewer A)
>
> To my knowledge, one of the first (if not the first) work to apply guided fuzzing to test complex software like compiler optimizations. (Reviewer B)

봉준호 감독은 <기생충>으로 아카데미상을 받았을 때, 우상인 마틴 스코세이지 감독 앞에서 그의 말을 빌려 수상 소감을 전했다.
> 가장 개인적인 것이 가장 창의적인 것이다

유명한 사람이 하는 것, 요새 유행하는 것을 쫓는다면 쉽게 2류까지는 될 수 있을 것이다.
하지만 분야를 막론하고 창의적인 생각은 (가령, 영화 감독에게는 영화 주제) 남의 뒤통수에 있지 않은 것이 분명하다.
현재 맡은 일에 충실하면서 내 안의 자그마한 소리에 귀를 기울여야 누구도 발견하지 못한 색을 갖게 된다.

나만의 길을 개척해가는 수레바퀴는 멈추지 않고 돌아갈 것이다. 파고들면 들수록 세상에 나만 아는 비밀로 가득할 것이다.
가슴 벅차지 않은가? 세상에 나만 아는 비밀이 있다는 것. 그리고 곧 그 비밀을 모두에게 자랑스럽게 이야기해 줄 수 있는 기회가 있다는 것.
이번 연구를 통해 우리는 또 다른 비밀 하나를 발견하고 파헤치느라 설레는 중이다. 과학자는 이러한 비밀이 밑천이다.
과연 과학자만 그럴까? 시인 이상도 소설 <실화>에서 이렇게 말했다:
> 사람이 비밀이 없다는 것은 재산 없는 것처럼 가난하고 허전한 일이다.
