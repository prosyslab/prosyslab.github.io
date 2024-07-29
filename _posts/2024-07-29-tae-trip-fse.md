---
title:  나의 첫 남미 학회 탐방기
date:   2024-07-29
author: Tae Eun Kim
kor_author: 김태은
tags:
  - Trip
  - FSE2024
classes: wide
---

| ![](https://lh3.googleusercontent.com/pw/AP1GczPtDz7E2kjWBT45pae_DdCVskngFRJ_iEsqL4aGFaCXptBusq_mDPAg2cgRdM3k2MYyne1jns76YORpiE4-UrHs0qpzTfVqYKz7gp5aVP-8tTdEVPp9AfQS6X7KceHYr4DZjptVR6Fvt87InlBUPQW2=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>FSE로 떠나자! 왼쪽부터 최재승 교수님, 나, 허기홍 교수님, 그리고 최진수님.</b>|


<br/><br/>

# 들어가며
지향성 퍼징 연구를 하며 느꼈던 답답함을 담았던 논문인 "Evaluating Directed Fuzzing: Are We Heading in the Right Direction?<sup>[1](#evaldirfuzz)</sup>"을 발표하러 2024 FSE 학회에 참석하게 되었다.
이번 FSE는 브라질에서 열리기에 생애 첫 남미행에 올랐다.
미국은 몇번 가 보았지만 브라질은 체감상 두배나 멀었다.
비행 시간만 28시간, 집에서 숙소까지는 42시간이 걸린 대장정을 거쳐 브라질의 Porto de Galhinas에 도착했다.
평소와 달리 우리 연구실에서 이번 출장길에 오른 학생은 나 혼자였기에 조금은 더 무거운 책임감으로 여행기를 시작해보려 한다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNyXYhH_xeP30gFFdjrCAKe1ZIJW_grNNNYQeUTT1xlSL3HUiD50rq4-ON0ySDtcAwa5coTkGeL0qo3uBYoBJosVbLYX3PvzUp98lF9QiGgAnDhYcq1Vo7Tzd0rAr2rGiw4DSSnlIaW70ptciRVuhs4=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>긴 여행 끝에 도착한 숙소 현관. 피로가 눈 녹듯이 사라졌다</b>|


<br/><br/>


# 발표 이야기
발표 준비는 항상 어렵다. 쉽다면 이미 여러번 한 발표거나 제대로 준비를 안 한 발표가 아닐까 생각한다.
학회 발표가 처음은 아니지만 논문의 성격이 다르다 보니 마치 처음 하는 것처럼 새로운 경험이었다.


## 초안 만들기
내 첫 [논문](https://prosys.kaist.ac.kr/publications/sec23-slides.pdf)은 문제 정의, 해결 방법, 실험으로 이루어진 일반적인 논문이었다.
그러다보니 하나의 문제와 아이디어를 개념적으로 쉽게 설명하는 것이 관건이었다.
하지만 이번 논문은 기존 논문들이 실험 과정에서 놓치고 있었던 여러 문제를 드러내고 그에 대한 해결책을 제시하는 논문이었다.
따라서 하나의 개념을 설명하기보다는 여러 단계의 각 문제와 해결책을 나열식으로 설명해야 했다.
나열식 발표의 관건은 단조로울 수 있는 흐름에도 불구하고 청중의 흥미를 유지시키는 것이다.
이룰 위해서는 각 항목이 모두 재미있어야 한다.
그래서 최대한 재미있고 충격적인 예제를 많이 집어넣었다.

## 다듬기
이번에도 정말 많은 도움을 받아 발표 자료를 다듬고 연습했다.
자료 초안을 완성한 이후, 논문의 교신 저자로 참여하신 서강대학교의 최재승 교수님과 함께 1차로 자료를 검토했다.
리허설을 하듯 내가 발표하고, 피드백과 논의를 통해 발표 자료를 수정하는 방식이었다.
바쁘신 와중에 긴 시간을 투자해주신 최교수님께 감사드린다.

두번째로는 논문의 공동 저자이신 허기홍 교수님과 차상길 교수님, 그리고 각 연구실 학생들 앞에서 리허설을 진행하였다.
약 20명 정도의 청중 앞에서 발표를 하는 것 자체도 귀하고 소중한 경험이었지만,
학생들의 다양한 질문과 피드백은 예상 질문을 대비하고 발표 자료의 세밀한 완성도를 높이는 데 큰 도움이 되었다.
또한 교수님들의 피드백은 정말 큰 도움이 되었다.
허기홍 교수님의 피드백은 발표 자료의 가독성에 큰 도움을 주었고, 차상길 교수님의 피드백은 우리의 동기가 무엇인지 정확히 전달할 수 있도록 도와주었다.

마지막으로는 소프트웨어 재난연구센터 워크숍에서 발표를 진행했다.
한국어로 발표하고 시간도 더 여유있는 30분으로 실제 학회 발표와는 차이가 좀 있었지만
100명에 가까운 청중 앞에서의 발표, 처지지 않게 흐름을 끌고 가는 연습, 그리고 사람들의 반응과 질문을 살펴보는 것이 매우 의미있었다.
특히 유신 교수님 연구실의 강성민 박사님이 주신 질문과 이주용 교수님, 최윤자 교수님이 주신 아티팩트에 대한 질문이 감사했고 또 도움이 되었다.

아이를 키우는데에는 한 마을이 필요하다는 말이 있지만 발표를 준비하는데에도 한 마을이 필요하다.
한 사람의 관점, 배경, 눈썰미는 너무 제한적이기 때문이다.
정말 많은 사람의 눈과 입과 손을 거쳐 내 발표 자료는 초안과 비교할 수 없을 정도로 완성도가 높아졌다.
이 자리를 빌어 도움을 주신 모든 분들께 감사드린다.

## 발표 직전
사실 조금 순탄치 않았다.
이번 FSE는 모든 논문 저자들에게 포스터 발표를 할 기회를 주어서 우리도 포스터를 준비했다.
그런데 문제는 포스터 세션이 30분이고, 내 발표 세션 직전으로 배정된 것이다.
순서가 반대였다면 정말 최고의 상황이었을 텐데 너무 아쉬웠다.
원래 발표를 할 때도 재밌게 들으셨다면 포스터 세션에 와주세요~ 라고 말하려고 했지만, 그럴 수 없게 되었다.
그래도 주어진 상황에서 최선을 다하기 위해 포스터를 붙이고 자리에 서 있었다.
생각보다 사람들이 많이 오길래 열심히 설명을 시작했다.
그러다 발표 시작 15분 전, 허기홍 교수님의 조언대로 발표 자료 확인을 위해 잠시 양해를 구하고 발표장으로 달려갔다.
문제가 없으면 바로 돌아와서 포스터 세션을 이어가려고 했지만 발표자들이 미리 제출한 해당 세션의 발표자료 파일이 모두 누락되어 있었다.
세션 체어가 문제가 해결되기 전까지 혹시 모르니 자리를 지켜달라 하였고, 어쩔 수 없이 포스터 세션은 그렇게 마무리 되었다.
그리고 어수선한 마음을 달래자마자 내 발표 순서가 찾아왔다.

## 발표
발표는 만족스러웠다.
실수도 없었고, 청중도 예상했던 것보다 많았다.
질문도 하나 있었고, 사람들도 끄덕거리며 들어주었다.
심지어 발표장엔 첫 지향성 퍼징 논문의 저자인 Abhik Roychoudhury 교수님도 계셨고 Andreas Zeller 교수님도 계셨다.
이렇게 네임드 교수님이 두 분이나 계신 상황에서 발표를 할 수 있다는 것은 굉장한 기회다.

하지만 이상하게 발표를 마친 후 아쉬운 마음이 들었다.
우선 야심차게 백업 슬라이드를 많이 준비했는데, 딱히 그것을 사용할 정도로 질문이 많지 않았다 (특히 "What's in my Artifact?"라는 제목의 슬라이드를 못 쓴건 상당히 아쉬웠다).
또 곰곰히 생각해보니 내가 기대했던 만큼의 보상을 받지 못했기 때문이었다.
그럼 난 뭘 기대했던 걸까? 기립박수라도 받았으면 기분이 좋았을까?
이제서야 생각해보니 나는 엉뚱한 보상을 바라고 있었던 것 같다.
진정한 학계의 보상은 내 논문을 인용하고, 내가 제안한 방법을 참고하고, 내가 만든 아티팩트를 활용하는 것일텐데
그런 것은 발표장에서 받을 수 없는 것이었다.
여기까지 생각이 미치자 약간의 반성과 함께 아쉬움을 털어버릴 수 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNE5RHmGzVsd0TJN_xag_Fq0SNMPbOenX7m0H_e0xtf8rM8v2HztuphVNk9K4XC97vNrRtX9PKjsi_T60khpReYlA603KmTBNpNqOFke6gosmUd8adHWI9FrPRlSe_vKVG__YaIJYddfmHjqiLQdnyoCg=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>발표 현장</b>|

| ![](https://lh3.googleusercontent.com/pw/AP1GczPtWu21sS010HqetnPwQoAgHRgeC01NrQZOPe03YJJpr2AYM6cnQweL3dDmKtf9BSwhaFmQ-280w0UeztNX7mCASrT0VHW1jRL-WO6AGojZ4_PmyMz21S-wxz9iD1_LcFZp0RLI94AwiE15z9_M88mL2Q=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>짧아서 아쉬웠던 포스터 발표</b>|


<br/><br/>


# 사람들

이번 학회 출장 일정에는 경북대학교 최윤자 교수님 연구실의 요엘이가 함께 했다.
요엘이도 논문을 발표하러 브라질에 가야 하는데, 나와 마찬가지로 연구실에서 학생으로는 혼자 가게 되어 숙소도 같이 쓸 겸 동행하기로 했다.
사실 지난 3년간 같은 연구센터에 소속되어 있어 그 동안 볼 기회는 많았지만 이번 학회 덕분에 동고동락하며 더 친해 질 수 있었다.

재미있게도 한국에 있어도 보기 힘든 사람들을 오히려 외국 학회에서 더 자주 볼 수 있다.
함께 연구를 진행하는 서강대학교의 최재승 교수님, 그리고 걸어서 10분 거리에 있는 카이스트의 강성민 박사님도 평소에 보기는 어렵지만 학회에서 만나 더 많은 이야기를 나눌 수 있었다. 

이번 FSE 에서는 새로운 만남도 있었다. USC의 William G.J. Halfond 교수님 연구실의 Zhaoxu Zhang과 Fazle Mohammed Tawsif였다.
Tawsif의 경우, 낯이 익어서 학회 단골 플러팅 멘트인 "우리 어디서 본 적 있지 않나요?"를 시전했는데 ([학회 네트워킹 실습 자료](https://goodtaeeun.github.io/assets/networking.pdf) 참고) 역시나
지난 4월 포르투갈에서 열린 ICSE Student mentoring workshop에서 만난 사람이었다.
그런데 이번에 알고 보니 이 친구와는 생각보다 인연이 깊었는데 그 시작은 22년 11월로 거슬러 올라간다.
LA에서 열린 CCS 출장의 마지막 날, 허기홍 교수님의 포닥 시절 동료인 Mukund 교수님의 초대로 USC에 방문하는 일정이 있었다.
이 때 소프트웨어 공학 분야 연구실의 학생들과 교수님들을 대상으로 우리 교수님이 발표를 하셨는데, 그 때 그 자리에 있었다고 한다.
서로 본 기억은 없지만 그 자리에 있었다는 사실만 각자 기억하고 있었다.
세상 참 좁다는 말이 이런 걸까, 이름도 몰랐지만 이번이 세 번째 만남이었다.
Zhaoxu는 점심을 같은 테이블에서 먹다가 알게 되었는데 알고 보니 Tawsif와 같은 연구실이었다. 이런 우연이!
나도 딱히 친구가 없고 이 친구들도 딱히 아는 사람이 많지는 않아 보여서 이 이후로도 보일때마다 같이 다녔는데,
이번 기회에 미국 대학원생의 삶이 어떤지 조금 더 알게 되었다.
앞으로 또 볼 기회가 있으면 좋겠다.


<br/><br/>



# New Faculty Symposium
행사 이름만 봐서는 신임 교수들만 모아놓고 무언가를 하는 것 같지만 사실은 누구에게나 열려 있는 워크숍이었다.
물론 프로그램은 신임 교수들을 위한 내용을 위주로 구성되었지만 대부분 대학원생에게도 도움이 되는 내용이었다.
기억에 남는 것은 Abhik Roychoudhury 교수님의 연구에 대한 발표 (Imagination in Research), 그리고 Denys Poshyvanyk 교수님의 연구 제안서 작성에 대한 발표였다.

### Imagination in Research
Abhik 교수님은 연구를 할 때 필요한 것 세가지를 언급했다.
첫 번째는 외부의 목소리를 듣는 것이다. 내가 풀고자 하는 문제에 대해 여러 사람의 의견과 관점을 들어봐야 이 방향이 맞는지, 이 연구가 꼭 필요한지 판단할 수 있다.
두 번째는 스스로에게 물어보는 것이다. 이 문제가 지금까지 안 풀렸는데, 내가 이걸 풀 수 있는 근거는 무엇인가? 가능성이 안 보이면 시작하지 말아야 할 수도 있다.
세 번째는 나 혼자 잘하고 마는 연구가 아닌, 남들도 잘 할수 있는 연구를 하는 것이다. 나 혼자 잘하고 마는 연구는 기존에 비해 X% 좋아지는 연구다. 기존에 없었던 새로운 연구는 남들도 잘 할 수 있는 기회를 제공한다. 예를 들어 지향성 퍼징의 첫 논문(각주)의 경우, 수많은 사람들이 지향성 퍼징 연구에 뛰어들 수 있는 길을 열어주었다.
이 중 두번째 포인트가 신선하게 다가왔다. 연구는 근거 있는 자신감이 필요하다.

### 제안서 쓰기
대부분은 한번쯤 들어봤던 내용이었지만 기억에 남는 것이 하나 있다.
좋은 연구 제안서는 하이 리스크, 하이 리턴이다. 따라서, 실패할 가능성이 있다는 것을 숨기지는 않되 그럼에도 불구하고 얻을 수있는게 무엇인지를 생각해보아야 한다. 굳이 제안서를 쓸 때뿐 아니라 연구를 할 때도 이런 것을 고려해보면 좋겠다는 생각이 들었다. 지금 하는 연구가 잘 안되더라도 나에게 남는 것은 무엇이지? 경험이 될수도 있고, 새로운 아이디어가 될 수도 있고, 만들어둔 프레임워크가 될 수도 있다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPDUb539O5_yURbYk98ikizgo3GbK9rcGfgm9L_8VGMbkvGFL7TVFoSevmAXzx7wGQAF1f_D5uv01Ja5I4JppSmTE9IHVi442OHqbMBp-7KL8RvL9d0ZoRW48CUdw43aoJfE5DS7tJyziTDHxdeMASV=w1295-h863-s-no-gm?authuser=0) |
|:--:|
| <b>Abhik 교수님의 발표</b>|



<br/><br/>

# 흥미로웠던 발표들

__Only diff is Not Enough: Generating Commit Messages Leveraging Reasoning and Action of Large Language Model<sup>[2](#omg)</sup>__ \
우수 논문상을 받은 커밋 메세지 자동 생성 연구.
기존 커밋 메세지 생성 도구들은 코드 변화 - 커밋 메세지의 관계를 학습하고, 이를 이용해 커밋 메세지를 생성한다.
그러나 단순히 코드 변화만을 기반으로 커밋 메세지를 생성하면 그 외의 맥락은 놓치게 되며, 애초에 사람이 만든 커밋 메세지 그 자체도 그리 양질의 정보가 아닐 수 있다.
따라서 이 연구에서는 코드 변화에 더해 다양한 맥락 정보를 LLM에 넘겨주어 더 좋은 커밋 메세지를 생성한다.
이때 여러 기존 도구들을 사용해 맥락 정보를 추출하는데, 그 정보는 다음과 같다.
수정된 파일 중 중요해보이는 파일 이름, 커밋 종류, 풀 리퀘스트 제목, 이슈 제목, 메소드 및 클래스 요약 정보.
참고로 메소드 및 클래스 요약 정보는 단순히 코드를 요약한 것이다.

사실 단순하게 보면 모을 수 있는 정보 최대한 다 모아서 LLM에 때려넣어 커밋 메세지 만드는 기법이라고 볼 수 있다. 그리고 발표자도 말하기를 현재 기법은 이렇게 정보를 물어다주는 도구들의 성능에 굉장히 의존적이라고 한다.
그럼에도 불구하고 도구 이름을 전지적 메시지 생성기(Omniscient Message Generator)라고 지었는데, 살짝 과장인것 같다.
논문을 자세히 읽어보지는 못했지만 우수 논문상 받았다고 하니 아마도 글을 잘 썼나보다.

__Towards Efficient Build Ordering for Incremental Builds with Multiple Configurations<sup>[3](#build)</sup>__ \
다양한 환경에서, 혹은 다양한 목적으로 사용되는 프로그램일수록 다양한 빌드 설정이 존재한다.
C 언어로 작성된 프로젝트를 빌드해본 사람이라면 `configure` 스크립트를 통해 다양한 옵션으로 빌드를 해본 경험이 있을 것이다.
만약 지속적 개발(Continous Integration) 환경에서 회귀 테스트를 위해 빌드를 자주 하는 경우, 이러한 다양한 빌드 설정을 효율적으로 관리하는 것이 중요하다. `make` 등을 통해 빌드를 한다면 빌드 설정이 바뀌더라도 이전 빌드 결과를 일부 재사용할 수 있지만, 얼마나 재사용할 수 있을 지는 각 빌드 설정에 따라 다르다. 따라서 각 빌드 설정 간의 거리, 즉 재활용이 가능한 정도를 고려해 빌드 순서를 결정하는 것이 중요하다.

이 연구에서는 각 빌드 설정 간의 거리를 계산해 효율적인 빌드 순서를 결정하는 방법을 제안한다.
이 때, 거리는 생성된 `Makefile`의 내용물을 비교해 계산하며, 순서는 먼저 가장 작은 사이즈의 설정으로 빌드를 한 후 그리디하게 그 다음 가까운 빌드를 진행하는 것으로 한다.

재미있는 점은 문제를 이렇게 정의하고 나면 이 문제는 TSP(Traveling Salesman Problem)로 귀결된다는 것이다.
TSP는 NP-hard 문제이기 때문에 문제의 크기가 커지면 최적해를 찾기란 쉽지 않다.
그래도 널리 알려진 문제인 만큼 동적 프로그래밍으로 푸는 등 보다 효율적인 방법이 존재하는데 왜 그렇게 하지 않았을까 궁금했다.
그리고 실험 대상으로 쓰인 프로젝트들의 서로 다른 설정의 개수가 어떻게 되는지도 궁금했는데 논문이나 발표에서는 따로 공개가 되지 않았다.
사실 발표 후 TSP 문제를 풀때 쓰는 휴리스틱을 안 썼냐고 물어봣는데 질문이 잘 전달되지 않은 것 같아 제대로 답변을 듣지는 못했다.


__Unprecedented Code Change Automation: The Fusion of LLMs and Transformation by Example<sup>[4](#tbe)</sup>__ \
Transformation by Example이란? 기존 예제로 학습된 코드변화 패턴을 적용하는 것. 단순히 말하면 자동 리팩토링이다.
이 연구는 LLM을 이용해서 더 유연하고 자연스러운 코드 변화 패턴을 적용하려고 하는 것.
이 때, 리팩토링의 기본은 의미의 보존이다. 보존되어야 하는 의미의 단위는 그때그때 다를 수 있다. 수정된 라인이 될 수도 있고, 함수가 될 수도 있다. 이 연구에서는 리팩토링 이후에 LLM이 생성한 테스트를 통해 원본 프로그램과 리팩토링된 프로그램의 동작이 같은지 검사한다. 

아무래도 이 연구는 대상 언어가 파이썬이라서 가능하지 않았을까 하는 생각이 든다.
파이선은 파이토닉하다는 표현이 있을 정도로 정답에 가까운 코드 작성 방식이 있기 때문에 자동으로 코드 변화를 적용했을 때 임의의 개발자가 이를 인정하기 더 쉬울 것 같다.

__Bounding Random Test Set Size with Computational Learning Theory<sup>[5](#pac)</sup>__ \
`The stopping problem: When can I stop my test?`
랜덤 테스팅을 할 때, 언제까지 테스트를 돌려야 할까?
이 연구는 랜덤 테스팅을 하며 생성되는 테스트의 분포가 일정할 때, PAC learning theory를 이용해 만든 공식으로 테스트 포화(test saturation)에 도달할 수 있는 테스트의 개수를 구하는 연구이다.
이 때, 테스트 포화란 관심있어하는 정보를 추가로 얻지 못하는 상태를 말한다. 커버리지가 더 이상 증가하지 않는 상태, 혹은 버그가 더 이상 발견되지 않는 상태 등.
그리고 여기서 사용하는 공식은 검증하고 싶은 가설의 사이즈, 정확도, 그리고 해당 정확도가 보장될 확률을 인자로 받아서 계산한다.

솔직히 모든걸 이해하지는 못했다. 공식의 의미라든지, 이게 어떻게 가능한 건지 등등. 그러나 개념적으로는 신기했고 발표도 잘 해서 이런 연구도 있구나 하는 마음으로 재미있게 들었다.
상당한 시간을 배경 설명에 할애해서 이해를 도왔기 때문이 아닌가 싶다.

다만 들었던 생각은 이렇게 구해진 필요한 입력 개수가 어차피 현실적으로 감당 가능한 비용보다 높으면 의미가 없지 않을까? 라는 것이었다.
상한선(upper bound)은 얼마든지 올라갈 수 있으니까 무한대라고 해도 틀린 말이 아니기 때문이다.
그리고 느낌상 지난 ICSE에 이성민 박사님이 발표한 논문<sup>[6](#coverage)</sup>과 비슷한 느낌이 들었다. 안 그래도 물어보니 후속연구를 함께할 계획이라고 하더라.


__A Quantitative and Qualitative Evaluation of LLM-based Explainable Fault Localization<sup>[7](#llmfl)</sup>__ \
강성민 박사님의 발표였다.
최근에 나도 오류 위치 추정 연구를 했던지라 더 재미있게 들었다.
이 연구는 LLM을 이용한 오류 위치 추정 방법을 제안하고, 이 방법이 얼마나 잘 동작하는지를 평가하는 연구이다.
오류에 대한 정보, 실패한 테스트와 그 결과를 LLM에게 주고 LLM이 대상 프로그램을 몇번 실행하며 오류 위치를 추정하게 한다.
그리고 추정 결과를 설명과 함께 제시한다.
논문이 된 만큼 성능은 당연히 기존 방법들보다 우수하다.
하지만 내 눈에 더 들어온 것은 유저 스터디 결과, 사용자들은 LLM이 제시한 설명을 굉장히 좋아했다는 사실이다.
단순한 에러 메세지가 아닌 풀어 쓴 설명이 사용자들에게 더 이해하기 쉽게 다가왔다는 것이다.
논문에 살짝 언급된 것처럼 설명을 교차 검증할 수 있도록 실행 결과와 함께 제시된다면 더 유용한 도구가 될 수 있을 것 같다.
따라서 LLM을 활용한 오류 위치 추정 방법은 그 정확성보다는 설명에 질에 더 주목해야 할 것 같다는 생각이 들었다.

이건 좀 다른 이야기인데, 이 연구는 자바를 대상으로 했으며 함수 단위로 오류 위치를 추정했다.
하지만 C 프로그램에서는 함수 단위는 택도 없으며 애초에 모듈화가 덜 되어있어 함수 단위로 한다 하더라도 LLM이 잘 못할 것 같았다.
강성민 박사님께 물어보니 C++에 대해서 해보긴 했는데, 역시나 잘 안된다고 한다.
과연 C 프로그램에서의 오류 위치 추정은 희망이 있는걸까? 도대체 어떤 기술이 필요한 걸까 궁금하다.

__Can GPT-4 Replicate Empirical Software Engineering Research?<sup>[8](#llmemp)</sup>__ \
재미있는 연구다.
GPT-4를 통해 관찰 연구 (Empirical Research)를 재시도할 수 있는가? (결론 미리보기: 못 한다)
관찰 연구는 데이터를 수집, 분석하여 결론을 도출하는 연구이다.
소프트웨어 공학 분야의 관찰 연구의 예로는 오류의 생애 주기를 추적하는 연구, 코드 리뷰의 효과를 분석하는 연구 등이 있다.
재시도라는 것은 기존 연구와 같은 방법을 다른 데이터에 적용하는 것을 말한다. 좀 더 구체적으로는 A 회사의 오류 생애 주기 데이터를 가지고 한 연구를 B 회사의 데이터에 적용하는 것이다.
이 때, 올바르게 연구를 재시도하려면 먼저 기존 연구에 내재되었던 전제들을 이해하고, 또한 기존 연구의 파이프라인을 이해해야 한다.
예를 들어, 풀 리퀘스트의 개수를 통해 개발자의 생산성을 측정하는 연구의 경우, 풀 리퀘스트의 개수가 개발자의 생산성을 반영한다는 전제를 깔고 간다.
하지만 1인 개발자가 풀 리퀘스트 없이 개발을 한다면? 이런 경우를 고려하지 않으면 잘못된 결론을 도출할 수 있다.
따라서 기존 연구의 전제를 이해하고, 이를 고려해서 재시도를 해야 한다.
이 연구에서는 GPT-4에게 논문을 주고 1. 이 논문의 전제를 정리해봐라, 2. 이걸 수행할 수 있는 파이프라인을 구성해봐라, 3. 그걸 코드로 구현해봐라 라는 과제를 주었다.

결론은 아직 GPT-4는 이런 연구를 할 수 없다는 것이다.
가장 큰 이유로 꼽히는 것은 소프트웨어 공학적 배경지식의 부족이다.
예를 들어 풀 리퀘스트에는 수정된 라인의 정보가 따로 표시되지 않는다고 하거나, GitHub와 V8이 비슷하다고 하는 등 상식적인 수준의 정보를 잘못 알고 있다.

사실 언젠가 대학원생이 하는 일을 인공지능이 하고, 대신 누가 인공지능을 얼마나 잘 지도하는지로 연구 실력이 갈리는 시대가 오지 않을까 상상해본 적이 있다. 인공지능이 못하는 건 사실 대부분의 대학원생도 처음에는 못하는 것들이지만 잘 가르치면 훌륭한 연구자가 되는 것처럼, 인공지능도 잘 가르치면 그럭저럭 연구를 할 수 있지 않을까?


<br/><br/>

## 학회 중 단상들

### 재현 가능한 연구
이번 Ideas, Visions and Reflections 트랙에 다음과 같은 두 논문이 있었다.
- __Reproducibility Debt: Challenges and Future Pathways<sup>[9](#repro)</sup>__
- __A Vision on Open Science for the Evolution of Software Engineering Research and Practice<sup>[10](#open)</sup>__

이런 논문이 나오는 이유는 무엇일까?
많은 연구의 결과가 재현 가능하지 않기 때문이다.
사실 연구 결과를 재현하는 것은 상당히 어려운 일이다.
실험 환경의 미세한 차이 (온도나 습도)에 영향을 받기도 하고, 실험자의 손 기술에 영향을 받기도 하며, 특정한 장비를 통해서만 재현이 가능한 경우도 있다. 우리 컴퓨터 분야는 이러한 제약으로부터 자유로운 편임에도 불구하고 여전히 재현 문제는 존재한다.

재현 안되는 연구가 많아지면 뭐가 문제일까?
후속 연구를 하기가 너무 어렵다.
어떤 분야의 첫 논문이 아닌 이상 기존 관련 기술들과 성능을 비교하는게 일반적이다.
그런데 막상 내가 기존 도구를 돌려봤는데 그들의 논문에 나온 것 같은 결과가 나오지 않는다면 어떻게 해야 할까?
내 실험이 잘못된 걸까 아니면 논문이 사기인 걸까? 알기 어렵다.
더 나아가 애초에 도구를 공개하지 않은 경우에는 어떻게 해야 할까? 그냥 믿어야 하는 걸까?
이런 어려움이 발생한다.

이런 재현성 문제의 저격수로 유명한 분이 바로 Andreas Zeller 교수님이다.
재현이 안되는 연구, 미심쩍은 연구, 성능은 잘 나오지만 정작 논문의 설명과 도구가 다른 연구 등에 대해 블로그에 글을 쓰거나 논문을 쓰기도 하신다.
개인적으로 이분의 [블로그](https://andreas-zeller.info/2019/10/10/when-results-are-all-that-matters-case.html)를 읽으면서 공감하고 같이 분노하기도 했다.
지난 ICSE때도 멀찍이서 보긴 했지만 이번에는 직접 만나서 이야기를 나눌 수 있었다.
좀 더 전투적인 이미지를 생각했지만 막상 얘기를 나눠보니 생각보다 더 조심스럽게 얘기를 하시는 것 같았다.
몰랐지만 지금까지의 저격 활동으로 인해 많은 공격을 받았다고 한다.
상대 저자들의 공격적인 이메일을 받기도 했고, 트위터에 공개적으로 비난이 올라왔단다.
재현 가능한 연구를 지향하고 또 연구 문화를 개선해가려는 연구자들이 받는 고통이 이렇게나 크다.

그렇다면 재현 가능한 연구를 하려면 어떻게 해야 할까.
A Vision on Open Science... 논문의 저자들은 여러 방안들을 언급하는데, 그 중에는 현재 아티팩트 배지 (Artifact Badge) 시스템의 개선이 있다. 많은 학회들은 아티팩트와 큰 상관없이 논문을 심사하고, 추후 아티팩트 공개 여부, 혹은 재현 여부에 의해 배지를 부여한다. 이 중 공애 여부에 대한 배지는 아티팩트를 공개 안 하는 것이 기본이고, 공개하면 특별히 더 잘한 것이라는 인식을 심어줄 수 있다. 따라서 아티팩트 공개를 원칙으로 하되 공개 여부에 의해 주어지는 배지를 없애고, 아티팩트의 품질에 따라 배지를 부여하는 것이 더 좋을 것이라고 한다.

나는 좀 더 급진적인 개선이 필요하다고 생각한다. 가장 강력한 제제 수단은 학회와 저널의 규정일 것이다.
연구의 재현 가능성을 염두에 두지 않거나 심지어 숨기는 경우, 그 이유는 무엇일까?
바로 출판을 빨리, 그리고 많이 하기 위해서이다.
따라서 그 출판의 길목에 검문소를 설치하고 재현성에 대한 요구를 강화해야 하지 않을까?
몇 가지 드는 생각이 있는데, 그 중 하나는 제보 시스템에 의한 종단 추적 심사 제도이다.
심사 당시에만 재현가능하도록 아티팩트를 만들거나, 심사용으로만 제작된 아티팩트를 공개하는 것을 막기 위해 제보 시스템을 도입하는 것이다. 이 경우, 아티팩트 심사는 1년 간격으로 두 번 이루어진다. 즉 제출 시점에 한번, 1년 후 한번 이루어지는 것이다. 이때 후속 심사는 재현성을 의심하는 제보가 들어온 경우로 제한하여 심사의 부담을 줄일 수 있다.
다음에 학회에 참석할 일이 있으면 타운홀 미팅에서 건의해보고 싶다.


### 학회란 무엇인가?
이번에 교수님들과 얘기하면서 저널과 학회의 차이를 좀 알게 되었다.
일반적으로는 저널이야말로 연구의 아이디어와 결과가 모두 탄탄한 완성된 논문이 실리는 곳이고,
학회는 보다 자유로운 분위기에서 다양한 아이디어를 논의하고 교류하는 행사라고 봐야 할 것 같다.
다만 우리 분야의 학회는 높은 경쟁으로 인해 다른 분야의 저널 수준으로 논문의 완성도를 요구하게 되었고 오히려 저널보다 더 높은 기준으로 심사를 하게 되었다. 이런 관행이 고려되어 학회 논문도 실적으로 인정되는 것은 좋지만, 한편으로는 저널 논문이나 학회 논문이나 비슷하게 되어버려 다른 분야에서 학회가 가지는 의미를 우리는 가지지 못하는 아쉬움도 생긴다.

재미있는 학회는 어떤 모습일까? 이것도 Andreas Zeller 교수님과 얘기중에 나온건데 마음에 들어 공유한다.
학회는 먼저 1차로 제안서처럼 아이디어와 초기 실험 정도만을 담은 논문을 심사한다.
즉, 학계의 사람들이 궁금해하고 가치있다고 인정한 연구를 시작하는 것이다.
그리고 2차로 구현과 실험을 완성하여 최종 제출을 한다. 이 때 2차에서는 따로 심사를 하지는 않는다.
여기에는 두 장점이 있다.
먼저, 심사는 결과와 무관하게 진행되므로 좋은 결과에 집착하지 않을 수 있다.
따라서 숫자 장난질이나 부정직한 실험 문화를 지양할 수 있다. 
둘째, 결과가 좋지 않았던 아이디어도 학계와 공유할 수 있게 된다.
결과 위주의 출판 문화는 잘되는 아이디어만, 혹은 어거지로 잘되게 만든 아이디어만 공유된다.
반면 안되는 아이디어가 무엇이고 왜 안되었는지에 대한 지식은 비밀스럽게만 전수된다.
하지만 둘 다 필요한 지식이기 때문에 모두와 공유한다면 더 빠른 속도로 연구가 발전할 수 있을 것이다.

물론 이 방법은 현실적으로 실현하기 조금 어렵긴 하다.
같은 기한 내에 모두가 연구를 마무리하기도 어렵고, 이런 방식의 학회 논문은 실적으로 인정해주지 않을 수도 있기 때문이다.
하지만 이런 즐거운 상상을 해보는 것은 자유 아니겠는가?


<br/><br/>

# 잡다한 이야기

### 아름다운 학회 장소
숙소가 해변의 리조트였고, 근처에 수영하기 좋은 해변도 있어 거의 매일 수영을 하고 코코넛을 하루에 두 통씩 마셨다.
일광욕도 잔뜩 해서 구릿빛으로 물든 채 귀국했다.
만약 내 논문 없이 학회에 왔다면 놀기에는 죄책감이 들고, 안 놀기에는 속 쓰려서 매우 힘들었을 것 같다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczOKnHW5KlesMOnZmjuFxrL7ciBRzoBtbOtiLXYkRomK-7ODBdtn6tXgjFh1BOM9gTIyg2xGpAIwH1igSoK-n4OSzGAw14En4koc0eXIgfgT-mvnmJVKr6D0ZQVouFPM1DfecXEB5SumQGwThAYLrVkh8Q=w1151-h863-s-no-gm?authuser=0) |
|:--:|
| <b>숙소 앞 해변</b>|


| ![](https://lh3.googleusercontent.com/pw/AP1GczNITBqtbkAY1uelCOfnuVEVt4IY--BzdV_4XY3C2BJZLlp8AxKYJUbKrkJSXO2rnmyjFrlTkR-g9KT-hFg8ir7JK0OyvcJFKJ9L7_8lrramO9EvgdvJU21hlCu2G7aj90b7_Py0oAnU_avWQdAoQHes=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>숙소 앞 수영장</b>|

| ![](https://lh3.googleusercontent.com/pw/AP1GczP3Le-x_yUOQiJjcNPA5Jg_UEewbeGI7KQ_V2jI2FjRKicKvjtvUbJhbT32aCReeUk_g9yt6D0iideDq88FZtlcysaTvuyh_rFcdQwcwIIrwm34u09ZAoXwOHAPJ6hkZ-g2aT_QTscg4pZE8v2w4X69=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>코코넛 한 통</b>|



### 선방하는 한국
우리나라는 제출 논문 수와 게제 논문 수 모두 6위를 차지했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNO2r5kn-2V7gz31bz0brhAnvedfF2s2zHlmoVEXhhF78YVJqVCestDCLBihiGo4XAhqSPh1AtfRXm3yvxgnrZ1neaWrn-8eNNeYT3pSSm_azQhx42sAiU2ExY-7EgSI2n_WV70FK9F93mFbI8uzoFF=w1151-h863-s-no-gm?authuser=0) |
|:--:|
| <b>논문 수 6위!</b>|


### 귀여운 발표 자료
첫째날 기조 강연은 Thomas Zimmerman의 발표였는데, 발표 내내 슬라이드에 매우 귀여운 일러스트가 하나씩 나왔다.
원래 고양이나 귀여운 것들을 좋아하는 분이라고 들었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNmFWEVSBT__Jp9oVfm-LBUNjaDQx7foClBDPjGDPUfI4xam8Dx_StjRRrizeqAAN8X63ZDqkecX014zD2U49AXi2XWs8j_mhD0HIyAb7KfGq343EgvIAkTV2Ixi3Qilxu6MH9fciRr86dn41_ja20N=w1151-h863-s-no-gm?authuser=0) |
|:--:|
| <b>귀염뽀짝</b>|


### 감동적인 음식
여태 참석한 학회 중 밥이 가장 맛있었다.
점심은 매일 호텔 식당에서 먹었는데, 적당히 로컬한 음식들도 있었고 맛도 좋았다.
미국에서 열린 보안 학회는 점심에 부리또 하나 주고 끝이거나 아예 안 줬었는데, 눈물이 날 뻔했다.
뱅큇 음식도 현지 해산물 요리로 아주 푸짐했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPG7ct3bjC0dJzxDUuemPSw6q_IBP30Qcr0bX5hX9nzN5kQXhtlWBdynQamsCYtFV-QOk7_dRqAWBclPxO1fyVFHa6OuVEXRpsU644nVhofV19cKmakEP8xAssR2TikmhVSio9rWznyrxKQPNWeZl5B=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>점심 식사</b>|

| ![](https://lh3.googleusercontent.com/pw/AP1GczNkc55bBvAO5BeiIMCvng_o8TZBkzbixEFWMM1IFZJWVOFkx2P6dLNwcsJwVU0Km15jtY0EBc0fSyE2dPkfBDDRD-AXxKxwYPFD7aGdwZqMOzkn6ptQaQ3zl4ZCNPD-dAuJGZu2EnjwVjbwzL9vsydW=w1151-h863-s-no-gm?authuser=0) |
|:--:|
| <b>뱅큇 식사</b>|


### 리셉션: 다양한 문화 행사
첫날 저녁 리셉션은 현지 공연팀의 무대로 시작되었다.
타운홀 미팅이 끝난 후 바로 그 장소에서 30분 정도 노래와 춤을 선보인 뒤 공연팀을 앞세워 모두가 리셉션 장소로 함께 행진하여 이동하는 방식이었다.
마치 축제에 온 것처럼 학회 참가자들이 골목을 가득 채우며 음악과 함께 이동하니 정말 기분이 좋았다.
리셉션 장소에 가니 우리나라 사물놀이 팀 같은 또 다른 공연팀이 각종 타악기를 연주하며 흥을 돋웠다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPhqOpeOUFW8PLcuGD9XpwXssRu64Y434DsrQs6kROijEqd0MCRFuow1ANNPjS7lI23I8YhyE2BMXuc48D_kdKZ5jPqljihw0itl8qg7ch6tpoApvh3KYxhK2CdFgKZRAQ4v4PvMTcIHIBVtzAxW0LD=w1295-h863-s-no-gm?authuser=0) |
|:--:|
| <b>공연</b>|


| ![](https://lh3.googleusercontent.com/pw/AP1GczNr1TYduZP3THqHi_zwJHi-TiUWocI6x2QDwp3cOMQMkVoaKV-gluxIdIblUvvvRl-fxLh1DIvyPHenw-lBsCV6n0CmnqFTTq4D6ciONZ-ECKAYXEdzlg6BjXVkdORO3g3iwqkMLnunyEMSP9BFZ2nv=w1295-h863-s-no-gm?authuser=0) |
|:--:|
| <b>행진하는 우리들</b>|


| ![](https://lh3.googleusercontent.com/pw/AP1GczM2FEVCupSd6ofbpS9DD1RbzsnrHBnc23PJdYoR6macbcXTUqKYCIMAQRKJmRUHMkrAe6xJ3NKdFAdjmYweKyGbsxcAc9nuEhBYAXYR_vsay7sLH0KeejILOgx9bELlKpACH2E15o4GrPLuklwwXUc8=w1530-h863-s-no-gm?authuser=0) |
|:--:|
| <b>브라질 사물놀이</b>|


### 뱅큇: 음식과 음악과 광란의 댄스파티
둘째날 저녁 뱅큇은 맛있는 식사와 함께 시작되었다. 먼저 시상식을 한 이후 현지 밴드와 가수가 무대에 올라 음악을 연주했다.
음악을 들으면서 식사를 마쳐가는 중 갑분댄이 되었다. 사람들이 하나 둘 신나서 앞으로 나오더니 밤 11시까지 무대 앞에서 춤을 췄다.
이 [영상](https://x.com/FSEconf/status/1814111081490444777)은 FSE 트위터에 올라온 당시 상황인데, 잘 보면 나도 나온다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczMfIlUSuz6A0h4LLDaDgESBTN8mT1Fk0NjUOINgwuuh0vok7q5jlgzptAnbNBscSeiHCVT1FKEvr3Hh6j9jIw_yT9gK31BhK9uncI59_2lfiJlsuMXnM66Nbjy2U_DWnvtvc7tIWLuGh4PlrcSXmEwn=w1295-h863-s-no-gm?authuser=0) |
|:--:|
| <b>밴드 연주</b>|

| ![](https://lh3.googleusercontent.com/pw/AP1GczM3VvlXQfprPHZVcGjREijVRH73IxsoC1XWLQKqeyDk4wZtsaeAKOtvsWTMn0X1kXGJqK95WNSxVfa9hpmVRuLWVQvfH6EL-V1_wH6jrvkJPHfWObPAkCu2Ik97ohlwaPm3o-BmbvhfJ1RxZChMcxPk=w1295-h863-s-no-gm?authuser=0) |
|:--:|
| <b>광란의 댄스 파티</b>|



### 10년 뒤, Test of Time Award를 위한 기념사진
이번에 Distinguished Paper Award를 못 받아서 아쉬운 마음을 달래며 허기홍 교수님과 함께 10년 뒤 Test of Time Award를 받기 위한 기념사진을 찍었다. 만약 10년 뒤에 Test of Time Award를 받게 된다면 이 사진을 꼭 발표 자료에 넣을 것이다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczOAfVAYAfRvI3qgzs0h06sP2Ajk6dBw4OTa2SUYPHYBDhHdMP6aLYrzg6V6IfOVpKE1irfXHz9qvkcdw5Xl-hbLzPCghRfZGk706n99TiMXKcT_zN9PKZsvLvetHJ1jOf2c6HupecLEFTPuLKD-QDJ3=w1151-h863-s-no-gm?authuser=0) |
|:--:|
| <b>10년 뒤를 기약하며</b>|

### 현지화 완료
피부를 태우고 현지 악세서리를 장착하고 사진을 찍으니 숙련된 관광객이 되었다.


| ![](https://lh3.googleusercontent.com/pw/AP1GczOXIaZKX75YRRy9VLemwlwc6Fxejlc6kDr0kcBZgG-jATOx-E8EBI34x9v_iThWiR2JV5Yib8OTCSpFmgQIqJLxLuik3q0RxkZMqjap1sH9QvIg59F1R95KBdLRyfH3O0dAu-CHKRyGt8lGgIpj60IA=w647-h863-s-no-gm?authuser=0) |
|:--:|
| <b>예아</b>|


<br/><br/>



# 돌아오며
훌륭한 지도 교수님과 공저자 교수님들과 함께 작업한 결과가 좋은 평가를 받아서 기쁘다.
나 혼자는 결코 하지 못했을 일이지만 많은 도움과 지도와 조언을 통해 논문을 쓰고 발표도 할 수 있었다.
함께 해주시는 교수님들께 감사한 마음으로 더욱 연구에 정진해서 앞으로도 좋은 결과를 만들어내고 싶다.
걱정 없이 출장을 다녀올 수 있는 우리 나라의 연구환경에도 감사한다.
필요한 만큼의 연구비와 비자 문제로부터 자유로운 환경이 보편적이지 않다는 것을 이번 출장에서 알게 되었다.
마지막으로 10일간의 긴 출장동안 집에서 기다려준 가족에게 고마운 마음을 전하며 글을 마친다.

<br/><br/>
<br/><br/>
<br/><br/>

---

### 각주

[<a name="evaldirfuzz">1</a>] Tae Eun Kim et al. "Evaluating Directed Fuzzing: Are We Heading in the Right Direction?" FSE (2024) \
[<a name="omg">2</a>] Jiawei Li et al. "Only diff is Not Enough: Generating Commit Messages Leveraging Reasoning and Action of Large Language Model" FSE (2024) \
[<a name="build">3</a>] Jun Lyu et al. "Towards Efficient Build Ordering for Incremental Builds with Multiple Configurations" FSE (2024) \
[<a name="tbe">4</a>] Malinda Dilhara et al. "Unprecedented Code Change Automation: The Fusion of LLMs and Transformation by Example?" FSE (2024) \
[<a name="pac">5</a>] Neil Walkinshaw et al. "Bounding Random Test Set Size with Computational Learning Theory" FSE (2024) \
[<a name="coverage">6</a>] Danushka Liyanage et al. "Extrapolating Coverage Rate in Greybox Fuzzing" ICSE (2024) \
[<a name="llmfl">7</a>] Sungmin Kang, Gabin An, and Shin Yoo. "A Quantitative and Qualitative Evaluation of LLM-based Explainable Fault Localization" FSE (2024) \
[<a name="llmemp">8</a>] Jenny T. Liang et al. "Can GPT-4 Replicate Empirical Software Engineering Research?" FSE (2024) \
[<a name="repro">9</a>] Zara Hassan et al. "Reproducibility Debt: Challenges and Future Pathways" FSE (2024) \
[<a name="open">10</a>] Edson Oliveira Jr. et al. "A Vision on Open Science for the Evolution of Software Engineering Research and Practice" FSE (2024)
