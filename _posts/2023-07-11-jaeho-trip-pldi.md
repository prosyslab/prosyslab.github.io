---
title:  2023 PLDI를 다녀와서
date:   2023-07-11
author: Jaeho Kim
kor_author: 김재호
tags:
  - Trip
  - PLDI2023
classes: wide
---


| ![](https://lh3.googleusercontent.com/pw/AP1GczNgeg-XKNd4IsLvoaTsD8h5JfNRpn3OIMDFpkZGWu8278WQg8naBwK3FYHYsvJYe55muo_NuXp27orJjQHdfMlsAEiwGPceZRXINJ2OlyfV1Gg3o7pvPhsd68T969XItillXe2RNog4Ky7ssQMD6Cxo=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>학회에서 만난 반가운 한국인들끼리 한 컷</b>|


# 들어가며

(내) 발표 없는 학회, 그것은 가히 대학원생이 누릴 수 있는 최고의 축제일 것이다. 물론 훌륭한 연구 성과를 거둔 뒤 학계의 구성원에게 이를 소개하는 자리가 있다면
그 역시도 최고의 영광이겠지만, 학계의 구성원으로서 다른 연구자들의 훌륭한 연구 성과를 신경쓰이는 일 없이 온전히 음미할 수 있는 기회는 흔치 않기에 이번 PLDI로의
출장은 정말 값진 경험이었다. 이러한 경험의 기회를 제공해 주신 허기홍 교수님께 감사의 말씀을 드리고 싶다. 그만큼 처음으로 수학여행을 떠나는 학생의 마음처럼 설렘과
긴장이 가득했던 PLDI에서 특히 인상깊었던 일들과 느꼈던 나름의 교훈을 공유하고자 한다.

# 단란한 튜토리얼, 즐거운 식사

본 학회 일정이 시작되기 전, 여러 주제의 튜토리얼들이 동시다발적으로 열려 원하는 주제의 튜토리얼에 자유롭게 참가할 수 있는 시간이 주어졌다. LLVM을 기반으로 새로운
언어를 만들어 보는 튜토리얼도 굉장히 흥미로웠지만, 더 새롭고 낯선 주제인 뉴로심볼릭 (neurosymbolic) 에 대해 다루고 이를 직접 구현해볼 수 있도록 Scallop
이라는 언어를 배울 수 있는 튜토리얼에 참여하게 되었다. 또 scallop을 만든 분들이 허기홍 교수님의 포닥시절 연구실 동료라는 소식에 더 관심이 가기도 하였다.

워낙 훌륭한 주제의 튜토리얼들이 동시다발적으로 열리고, 그 사이에서 뉴로심볼릭은 아직 PL 덕후들에게 거리가 있는 주제여서인지 Scallop 튜토리얼에는 참여한 사람이
많지 않았는데, 그것이 오히려 큰 이득이었다. 튜터들과 더 가까이서 맞춤형 설명을 들을 수 있었고, 덕분에 논문을 읽는 것만으로는 알기 어려운 디테일까지 체험하고
이해할 수 있는 시간이었다. 특히 이산적이고 구조적인 형태를 갖추는 정보들까지도 요소마다 수치를 부여해 해석적으로 다룰 수 있도록 하는 것이 가장 흥미로웠는데, 보통
프로그래밍 언어는 매우 이산적이고 구조적으로 정의되어 마치 블록을 쌓듯 다뤘어야 했기에 이를 해석적으로 다루는 것이 어떤 의미를 가질지 깊이 생각해볼 수 있는 기폭제가
되었다.

튜토리얼이 단란했던 만큼, 함께 참여했던 태은님의 용기 덕분에 이 단란한 분위기를 이어가 점심 식사까지 튜터 분들과 같이 즐길 수 있게 되었다. 물론 대단히 영어를
못하는 내가 적극적으로 대화를 이끌어나가진 못했지만 영잘알 태은님과 친절한 튜터분들, 또 쾌활한 친구 Mayank 덕에 연구 내적으로, 외적으로 모두 충만한 이야기를
많이 들을 수 있었다. 특히 허기홍 교수님의 포닥시절 연구실 사람들, 즉 UPenn의 Mayur Naik 교수님 연구실 사람들이라는 공통분모 덕에 어디서도 듣지 못할 흥미로운
이야기들을 잔뜩 들을 수 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNZsISF-99zKQ4QSbDUcqtR1TyJB7ceOx9sRk8c5JfdKzeAWlONQZzyqt77SemWmy7qLbkKY3VUfhx9lYt2d4rE-LJ4qhy-_kA18zLlBZUHt5lXnBhKbP7ygAo5Ht5W27v3TmOXbC_uNPTiK5Gl9Ufy=w1080-h810-s-no-gm?authuser=2) |
|:--:|
| <b>왼쪽부터 Mayank, 태은님, 나, Jiani, Ziyang, 참고로 사진은 Jiani로부터 본인이 직접 전달받은 것이다</b>|

# 지구 반대편에서도 비슷한 고민들을 품고 있다

튜토리얼 이외에도 본 학회가 시작되기 전날 여러 워크샵이 열려 참여할 기회가 있었는데, 우리는 그 중 프로그래밍 언어론 분야에 새로 몸담게 된 학생들을 대상으로 멘토링을
진행하는 PLMW (Programming Languages Mentoring Workshop) 에 참여하게 되었다. 이번 PLMW는 프로그래밍 언어 학계 및 산업계 석학들의 경험과 생각을
들을 수 있는 강연 위주로 진행되었다. 

워크샵에서 가장 인상깊었던 부분은 이미 훌륭한 성과를 이루어내 학교 혹은 기업에서 본인의 능력을 펼치고 있는 패널들을 모시고 학생들이 앞으로의 커리어를 쌓아나가는 데
어떤 마음가짐을 가지고, 어떤 경험을 쌓아 나가야 할지 이야기를 들어볼 수 있었던 패널 세션이었다. 초반 꽤나 경직되고 어색한 분위기에 선뜻 질문하지 못했던 학생들도,
패널들의 솔직하고 구체적인 경험담과 진심을 들으니 차츰 더 많은 고민들을 공유하게 되어 활발한 이야기를 나눌 수 있었다. 

학생들의 고민은 크게 다르지 않았다. 사실 어떤 특별한 질문들이 있었는지 기억도 안 날 만큼 평범했고, 그만큼 어찌 보면 뻔하다고 느낄 법한 이야기들이 오갔다. 그 점이
오히려 특별했다. 사람들마다, 각자의 성격에 따라 다르겠지만 보통 본인의 진로와 적성에 고민이 있을 경우 갈수록 답이 보이지 않고 어디에도 본인과 같은 상황에 놓인
사람이 없는 것처럼 느껴질 때가 있을 것이다. 그러나 명심해야 할 것은, 거시적인 관점에서 대부분의 고민은 이미 겪어본 사람이 있으며, 나름의 해결책 혹은 선택의 결과가
데이터로 쌓여 있다는 것이다. 이리 당연한 사실을 새삼 느끼게 된 것이 PLMW에서 가장 큰 수확이 아닐까 한다.

# 전설을 만난 본회의 패널 토론

이번 학회는 PLDI 단독으로 진행된 것이 아니라, FCRC라는 이름으로 시스템 및 컴퓨터 구조 관련 학회 ISCA와 여러 위성 학회들이 함께 열려 매우 큰 규모로 진행되었다.
이에 따라 본회의 세션이 매일 따로 열렸고, 본회의 세션에서는 주로 일반적인 컴퓨터과학이라는 분야 측면에서 지금까지 해낸 성과를 함께 공유하고 우리가 직면하고 있는
가장 큰 과제가 무엇이며 이를 어떤 방향으로 바라보고 해결해야 할지 각 분야의 석학에게 듣는 자리가 마련되어 있었다.

솔직히 대부분의 발표는 집중해서 듣지 못했는데, 워낙 모든 분야를 아우르거나 프로그래밍 언어 분야 이외의 지식을 알아야 이해할 수 있는 내용이 많이 나오기도 했고,
굉장히 큰 회의장에서 진행되어서인지 발표하셨던 몇몇 분들도 긴장하여 말을 더듬거나 방언이 터지는 등 영알못에게 가혹한 환경이었던지라 시차 적응에 힘들어 하고 있던
시점에서 감명깊게 이야기를 흡수하기에는 무리가 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPIdhMYAAkwaDoW_gnwTDOKd0Tnojv3kOmsxMsGxbEb8eXbQoUq_69VLFkX6vCVP6kuzWor34Le_1dh6GP63wXIZ5hvMrKfyFyp9cFmPMpesWatKtWiMbibQuendGUj3abJsUXgR4j0dziMWkFjCceg=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>앞에서 세 번째 줄에 앉아 직접 촬영한 Steele의 모습. 우수에 찬 듯한 표정이다</b>|

그럼에도 학회 일정을 통틀어 가장 흥분되었던 일정은 본회의 세션 중 하나였는데, 바로 프로그래밍 언어 분야의 살아있는 전설 중 하나인 Guy L. Steele Jr가 패널로
참여했던 토론 세션이다. Steele 외에도 컴퓨터과학의 각 분야에서 현재 선두를 달리고 있는 최고의 석학들을 모시고 컴퓨터과학 전반에 걸쳐 지금까지 어떤 발전을 해왔으며,
앞으로 어떤 것에 주목해야 할지 이야기 나눠보는 세션이었다. 과거의 컴퓨터가 추구했어야 했던 효율 (efficiency) 과 지금 추구해야 할 효율에는 차이가 있다는 이야기
등 본질을 꿰뚫는 다양한 이야기가 오갔는데, 그 중에서도 프로그래밍 언어의 문법 및 의미를 엄밀히 정의하는 데에 많은 시간을 쏟은 Steele이 기계학습 기법을 활용한
프로그래밍에 대해 어떻게 생각하는지 들을 수 있어 감격이었다. 그는 인공신경망도 결국 기호로써 명확히 표현 가능하게끔 프로그래밍할 수 있어야 한다는 말을 하였는데,
이 때 뉴로심볼릭이라는 단어를 직접 사용한 것이 매우 인상 깊었다.

# 기억에 남는 세션 및 발표들

PLDI 본 학회에서 특히 기억에 남았던 세션에 대해 소개하고, 그 중에서도 인상깊은 발표가 있었다면 느낀 바를 이야기하고자 한다.

## 최우수 논문 세션

이번 PLDI는 최우수 논문 (distinguished papers) 세션을 따로 만들어 대부분의 최우수 논문들의 발표를 한 번에 들을 수 있도록 하였다. 본 학회가 시작됨과
동시에 진행된 세션인 만큼 대부분의 참석자들이 모여있는 자리에서 올해의 프로그래밍 언어 연구들에는 어떤 것들이 있는지 볼 수 있는 시간이었다.

분야를 나누지 않고 뽑힌 최우수 논문들의 발표를 한 번에 보고 있자니, 발표들 사이의 공통점을 발견할 수 있었다. 먼저 연구에서 해결하고자 하는 문제가 명확하다는 것과,
좋은 의미로든 나쁜 의미로든 의외로 주요 아이디어는 쉽고 간단했다는 것이다. 물론 발표만을 듣고 이해하려는 입장에서 각 연구의 숨겨진 고난과 역경을 모두 알 수는 없는
노릇이지만, 그만큼 과학적인 발견 또는 성과에 해당하는 부분 만큼은 어떤 어려운 연구도 분야 관계없이 누구든 이해할 수 있을 만큼 명확하고 간결해질 수 있다는 사실이
한 명의 연구자로서 설레는 점이었다.

### CryptOpt: Verified Compilation with Randomized Program Search for Cryptographic Primitives<sup>[1](#cryptopt)</sup>

| ![](https://lh3.googleusercontent.com/pw/AP1GczOGV2JMruo11BkzVTNxtCYVWIxl2EISNVe9hes2RWubInpLXpkhL-fgW9Y8bsgK9ZMXb4v7p_xY1L_YhgxauuXBKJeLhdATPD_fdBuufD185MDVICQ3vK_ozZVijq7yeB_gIr5GcjCAcV1zo5bHvalV=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>CryptOpt 발표</b>|

들은 발표 중 기억에 남는 것을 하나 꼽자면, 기초적인 암호화 알고리즘을 대상으로 하는 검증된 컴파일 방식에 대해 연구한 CryptOpt라는 발표였다. CryptOpt는
기존의 컴파일러들보다 뛰어난 최적화를 하기 위해 프로그램 무작위 탐색을 통해 컴파일된 프로그램의 크기를 효과적으로 축소하였는데, 무작위 탐색으로 찾은 후보 프로그램이
기존의 프로그램과 완전히 같은 의미를 가지는지 확인하기 때문에 성능과 안전성 모두를 챙길 수 있었다고 한다. 최적화 아이디어가 간단해도 너무 간단해 특히 기억에 남았는데,
예전 마르코프 연쇄를 활용하여 gcc의 -o3 최적화보다도 더 뛰어난 최적화 성능을 보이는 STOKE<sup>[2](#stoke)</sup>라는 툴을 선보인 연구가 떠올랐다.

## 기계학습 세션

프로그래밍 언어를 다루는 분야가 전통적으로 그래왔듯, 논리적으로 딱 떨어지지 않는 것에 큰 문제를 느끼는 사람들이 많았다. 그래서인지 기계학습 세션임에도 모델로부터
그럴듯한 결과물을 만들어내는 데에 의의를 두는 연구보다는 그 결과물을 더 엄밀히 정의하고 활용할 수 있도록 하는 연구, 기계학습 그 자체를 엄밀히 정의하고 기계학습
모델에서의 버그를 정의하여 이를 자동으로 수정하려는 연구, 또는 검증 과정을 거쳐 결과물을 신뢰할 수 있도록 하는 연구가 대부분이었다. 그 중 가장 기억에 남았던 발표
하나를 소개하고자 한다.

### Scallop: A Language for Neurosymbolic Programming<sup>[3](#scallop)</sup>

| ![](https://lh3.googleusercontent.com/pw/AP1GczOm4fIfJYA_vy4lC9_gHDWl-6beOWPO7tmHDk_E5xiprc0ADq9Jz24ZCbrUs3COwfdNyhwtr1gZsyfBWsSvIDe3TXmtgnZlamoEyfBy7dNJLeKlcuijXwg5avRZIZIFHCZ6ar-XjABpRJPsG-t54wTs=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>Scallop 발표</b>|

튜토리얼로 먼저 접했던 것인데, 연구 발표로써 다시 들으니 더욱 새로웠다. 뉴로심볼릭이라는 단어를 처음 들었을 때 떠올릴 수 있을 가장 직관적인 방식으로 뉴로심볼릭을
활용하는데, 기계학습의 과정에서 기호와 규칙으로 설명 가능한 부분은 기호와 규칙으로 대체하여, 입력으로 주어지는 데이터와 최종적으로 얻어내고 싶은 출력 사이에 학습을
위한 모델과 규칙을 적용하기 위한 모듈을 파이프라인처럼 연결하는 구조로 더 효율적이고 믿을만한 기계학습을 이끌어 낸다는 것이다.

학습을 위한 모델이 최종 출력을 직접 내놓는 것이 아니라, 모델이 내놓는 구조적 정보로부터 정통적인 방식의 알고리즘을 적용하여 최종 출력을 얻어내고, 그 출력을 이용해
지도학습 (supervised learning) 을 한다는 컨셉은 기계학습에서 알고리즘을 활용한 지도 (algorithmic supervision) 라는 이름으로 이미 존재하는데, 이 때
전통적인 방식의 알고리즘이 들어가야 하는 자리에 관계 논리라는 훌륭한 논리 도구를 활용한 프레임워크를 넣음으로써 개발자가 모델에게 학습시키고자 하는 데이터의 구조적
정보와 규칙을 직접 정의해 주면 그에 맞게 학습하는 모델을 만들 수 있도록 해준 것이다. 이 연구에서는 Scallop이라는 이름의 언어를 만들어 실제로 개발자를 위해
서비스하고 있는데, 언젠가는 Scallop 프로그램 (즉 관계 및 규칙에 대한 정의) 를 자동으로 합성하여 개발자가 별다른 노력을 하지 않아도 충분히 효율적이고 신뢰 가능한
학습 모델을 완성할 수 있도록 하는 연구를 진행해 봐도 재미있을 것 같다.

## 합성 세션

합성 세션은 크게 두 방향의 연구로 나눌 수 있었는데, 전통적인 프로그래밍 언어 분야에서의 프로그램 합성 기술을 더 발전시켜 주어진 조건을 완전히 만족하는 프로그램을
더 효과적으로 생성하는 연구와, 컴퓨터 과학에서의 어떤 문제를 새롭게 정의하여 이를 설명 혹은 해결할 수 있는 언어를 새로 정의한 뒤 기존의 프로그램 합성 기술을 토대로
본인들이 정의한 언어로 작성된 프로그램을 생성해 내면 그것이 문제의 해결 방법이 되는 연구가 있었다.

프로그램 합성 기술을 발전시킨 연구들 역시도 각자의 킥이 있고, 그 킥이 의외로 간단하거나 이미 알고 있는 기법으로부터 발전해 온 것이 보여 재미있었는데, 전체적으로는
어떤 문제를 해결하기 위해 특수 목적 언어 (domain specific language) 를 직접 정의하고, 이를 자동으로 합성함으로써 문제를 해결하는 연구들이 굉장히 흥미로웠다.
마치 프로그래밍 언어라는 장인의 검을 나만의 숫돌로 갈아 새로운 적을 처치하는 느낌이 들어, "프로그래밍 언어 연구자라면 이런 방식으로 세상을 구해야지" 라는 생각까지
들었다.

## 분석 및 최적화 세션

이 세션은 분석 자체보다는 최적화에 조금 치우쳐져 있는 세션이었는데, 그래서 처음에는 이 세션을 선택하여 참석한 것을 후회했지만 의외로 듣다 보니 고수준 언어에서의
최적화를 다루는 연구도 많았고, 개념의 생소함에 비해 이해의 속도와 흥미가 컸던 세션이었다.

### Better Defuctionalization through Lambda Set Specialization<sup>[4](#defunc)</sup>

| ![](https://lh3.googleusercontent.com/pw/AP1GczMB_uZzNc_ZrnQ-8emYCkYSMISKJcqwhenLCpu2Z1bWewRENozh8cy9-PbMpEMxozcJy-jbbeb0UsaUP0yXDLUTrVWNsAn-rZbND0VPck6aEBknMrFNyCfyDk9rsCiqhdHw1WsqroAzELnUE_wBEzhz=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>Better Defunctionalization (이하생략) 발표</b>|

이 연구에서는 정말 처음 들어보는 함수 해체 (defunctionalization) 를 효과적으로 하기 위해 익명함수를 더 특별히 다루는 내용을 소개하였다. 생소하디 생소한
개념의 연속이었음에도 이 발표가 기억에 남을 수 있었던 것은 그만큼 발표자들이 발표를 재미있게 구성하였기 때문이다. 발표자들이었다. 한 명의 발표자가 아닌 두 명의
발표자가 나와 서로 대화를 주고 받듯 진행을 하였는데, 그 덕에 비기능화가 어떤 개념인지, 그래서 익명함수를 왜 특별히 신경 써주어야 하며 본인들의 연구에서는 그래서
어떻게 신경 써주었는지 물 흐르듯 머리에 들어올 수 있었다. 기회가 된다면 관련 공부를 더 해서 함수형 언어를 위한 최적화 연구를 해보고 싶다는 생각이 들 정도였다.

# 마무리하며

처음이라 정신도 없고 시차적응과 영어 이슈로 최상의 경험을 하지는 못했을지라도, 학회 전체를 관통하는 여러 생각들이 연구자로서의 나로 하여금 원동력을 만들어 주게 된
것 같다. 대학원생들에게 학회란, 내 발표가 없거나 적어도 끝난 이후부터는 최고의 전력 공급원이지 않을까 한다. 이번 학회를 경험하면서 가장 크게 느낀 부분들은 다음과
같다.

학회의 이름이 프로그래밍 언어의 설계와 구현 (Conference on Programming Language Design and Implementation) 이어서인지, 거의 모든 발표가 그
끝에 본인들의 연구 내용을 실제로 구현한 툴을 직접 사용해 보거나 실험 데이터를 확인할 수 있는 사이트를 알려주는 식으로 마쳐졌다. 그저 "나 연구 잘했어요" 로 끝나는
게 아니라, 정말 본인의 결과물을 자신있고 투명하게 공개한다는 느낌을 받아 신선했고, 또 내 연구도 떳떳하게 구현체를 자랑할 수 있을 만큼 예쁘게 코딩하고 싶다는
욕심이 생기기도 하였다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPqXcZxLPOogEadJnLO5IsmW3y0xEPQcsX_q_mpxZN7D-p9Qlt0hCoexfNZ-iMsNbH_FD_2eoIYowjc51app4mPOyI4_oyrz5qDqE_IItVbRNfTevAgoJTEDQd5iEJTuxdYHU8ZcaFOBiBm-ECNyZ0B=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>마지막 슬라이드에 본인들의 툴을 사용해볼 수 있는 사이트를 QR코드로 띄워놨다</b>|

마지막으로, 이번 학회에 참여할 수 있도록 기회를 주신 교수님과, 영어를 못해도 너무 못하는 내가 다양한 사람들과 그래도 조금씩 대화를 나눠볼 수 있도록 적극적으로 나서
주신 태은님께 감사하다. 나 혼자만으로는 쉽사리 경험하지 못할 일들을 이렇게나 많이, 짧은 시간동안 경험할 수 있었던 것은 모두 주변 사람들의 선의가 있었기 때문이다.
늘 가슴에 새기며 나 역시도 누군가에게 선의를 베풀 수 있고, 또 도움이 되는 사람이 될 수 있도록 하고 싶다.

<br/><br/>
<br/><br/>
<br/><br/>

----


### 각주

[<a name="cryptopt">1</a>] Joel Kuepper, Andres Erbsen, et al. "CryptOpt: Verified Compilation with Randomized Program Search for Cryptographic Primitives" PLDI (2023) \
[<a name="stoke">2</a>] Eric Schkufza, Rahul Sharma, and Alex Aiken. "Stochastic Superoptimization" ASPLOS (2013) \
[<a name="scallop">3</a>] Ziyang Li, Jiani Huang, and Mayur Naik "Scallop: A Language for Neurosymbolic Programming" PLDI (2023) \
[<a name="defunc">4</a>] William Brandon, Benjamin Driscoll, et al. "Better Defunctionalization through Lambda Set Specialization" PLDI (2023) 