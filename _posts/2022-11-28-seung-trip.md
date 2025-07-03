---
title: 2022 ACM CCS 학회를 다녀와서
date: 2022-11-28
author: Seungwan Kwon
kor_author: 권승완
tags:
  - Trip
  - CCS2022
classes: wide
---
11월 7일 부터 11월 11일까지 ACM CCS 2022가 미국 LA 다운타운에서 열렸다. 같은 연구실의 우석님의 논문이 채택된 덕분에 함께 CCS를 방문할 기회를 얻게 되었다.

## LA 도착
미국에는 하루 일찍, 11월 6일 오후에 도착하였다. LA 공항의 성조기가 미국에 왔음을 실감케 했다.

![](https://lh3.googleusercontent.com/pw/AP1GczPB0eaIkJirlyQCDeXQceCu2ocsTNHsfwpiUK0R83bHOdDOdmzxQ8jjKkoinh3mgxOOGjS_q4O4eimU-O1pKDx6j-SzUcxiUuLZTCqTvA4nq4DiZ3AxtwgfMNGIUsiacyK8qdagbv_2A7EIwqYvb-A=w651-h868-s-no-gm?authuser=2)

도착한 날의 날씨는 무척 좋았다. LA 날씨라고 하면 흔히 상상하는, 맑고 파란 하늘, 강한 햇살이 우릴 맞아주었다. 그러나 장시간의 주행과 비행으로 모두 피로하였기에, 곧장 호텔로 향했다.

호텔은 LA의 Omni Los Angeles 호텔로, 금융 회사의 빌딩들이 즐비한 도심과 조금은 정겨운 구도심의 경계에 위치했다. 이 두 지역은 1901년에 만들어진 엔젤스 플라이트라는 케이블카로 연결되어 있는데, 지대간 고저차가 꽤 있어 영화 기생충을 연상시키기도 했다.

![](https://lh3.googleusercontent.com/pw/AP1GczO96umXwzuWWzBQVQOqoiAvFncvsg5YbTrlF_4CRc74slwuBKVu5SvcjEiVx6j1QWVUS3fw5zPQJJ1eJ8N3Hyx837iB_dg6zezLDd6oSTRKQPkBWChub55GyQccDvPuX_qsyDbUVXw234Fc5L3mdD0=w651-h868-s-no-gm?authuser=2)

객실은 해질 무렵의 풍경이 인상적인 곳이었다.

![](https://lh3.googleusercontent.com/pw/AP1GczMNehdGrqAchfUbIsUoSN7p5oJ1TpNkMVDGyJvr_UgHwE2EJVgmQFB9ah8X5UXmszHdsAI7hZsNOsqk-1059D1SakuLBJICKo5f3eQzzYta4cwJaByJssFgPadgbJF7-EYPBhX9no1Ry6RUAif29y8=w651-h868-s-no-gm?authuser=2)

## 학회 참석

학회는 월요일과 금요일은 워크숍, 화요일부터 목요일까지는 본 행사로 구성되었다.

![](https://lh3.googleusercontent.com/pw/AP1GczPHONMKoY74jDDA8STwLfWwldjhXeozRh7lnxVUHCmi_YiV9WqN3JavaBxeVau8coBgNL_e85PDnzIebstu6ZXa4ot2iR0IWx5unpHwQsCPqS0ndlCWBnI4nQ9J59Na0tTw1VfNA6AHZu6nryQw2og=w651-h868-s-no-gm?authuser=2)


보안 학회이다보니 분야가 넓어 흥미롭게 들을 수 있는 세션이 많지는 않았고, 퍼징 세션과 소프트웨어 취약점 탐지 세션을 집중해서 들었다. 이중 관심있게 들은 발표를 정리해본다.


### JIT-Picking: Differential Fuzzing of Javascript Engines<sup>[1](#JitPicking)</sup>

많은 현대의 자바스크립트 엔진 (JS 엔진) 들은 크게 인터프리터와 JIT 컴파일러로 구성된다. 이 연구는 그 중에서 JIT 컴파일러의 오류를 더 잘 찾을 수 있도록, 기존의 퍼징 연구를 개선하였다.

연구에서 사용한 방법은 인터프리터로 함수를 실행한 결과와 JIT 컴파일된 함수를 실행한 결과를 비교하는 것이다. JIT 컴파일러에서 잘못된 최적화가 일어났을 때, JS 엔진이 비정상 종료되기 보다는 함수의 반환 값만 바뀌는게 더 일반적이므로, 효과적인 접근일 것이다. 실제로도 꽤 많은 버그를 찾았다고 한다.

흥미로웠던 것은 나 또한 최근 이 분야에 관심을 갖고 있지만, Usenix 2023에 FuzzJIT이라는 굉장히 유사한 논문도 채택되었다는 것이다. 인터프리터와 JIT 컴파일러를 비교하여 오류를 찾자는 아이디어가 같았고, Fuzzilli라는 퍼징 프레임워크 위에 이를 구현하였다는 점도 같았다. 말하지 않아도 서로 비슷한 생각을 하고 있다는게 신기했고, 또 굉장히 경쟁이 치열한 분야라는 느낌도 받았다.

### Non-Distinguishable Inconsistencies as a Deterministic Oracle for Detecting Security Bugs<sup>[2](#NDI)</sup>

핵심 아이디어는 어떤 함수의 두 실행 경로가 프로그램의 상태를 다르게 변화시키는데, 외부에서 이를 구별하지 않으면 버그로 이어질 수 있다는 것이다. 예컨데, 함수의 반환이 어떤 객체의 주소 또는 Null일 수 있다면, 그 반환 값을 참조하기 전에 반드시 검사가 이뤄져야 한다는 것이다.

아이디어는 직관적인데, 찾고자 하는 속성이 너무 일반적이어서 오탐이 많을 것 같다는 생각이 들었다. 실험은 4개의 소프트웨어 (OpenSSL, FreeBSD, httpd, PHP)를 대상으로 이뤄졌는데, 51개의 버그를 찾았다고 하며, 오탐률은 46% 정도를 기록했다고 한다.

### DirtyCred: Escalating Privilege in Linux Kernel<sup>[3](#DirtyCred)</sup>

이 발표는 커널 익스플로잇의 일종인 권한 상승에 관한 것이었다. BlackHat USA에도 발표되었으며, 패치되지 않은 대부분의 최신 리눅스에 적용된다.

연구의 아이디어는 일반 사용자의 `cred`를 루트의 것과 바꿔치는 것이었다. 리눅스에서는 각 프로세스마다 권한을 기록해둔 `cred`구조체를 힙 메모리에 저장해두고 있는데, 커널의 힙 관리 메커니즘의 취약점을 이용하여, 일반 사용자의 것을 루트의 것으로 변경할 수 있다고 한다.

발표를 들었을 때는 이 공격을 안정적으로 성공시키기가 매우 어려워 보였다. 그래서 기술적으로 자세한 설명을 기대하고 있었는데, 발표 시간이 10분으로 워낙 짧아 궁금한 내용이 생략된 것은 조금 아쉬웠다.

### TRACER: Signature-based Static Analysis for Detecting Recurring Vulnerabilities<sup>[4](#Tracer)</sup>

같은 연구실의 우석님 발표였다. 연구의 아이디어는 과거 버그들의 정보를 활용하여, 정적 분석 결과의 품질을 개선하는 것이었다. 국내 워크숍 및 내부 세미나를 통해 우석님의 발표를 숱하게 들었는데, 개인적으로는 이번 발표가 가장 좋았다.
![](https://lh3.googleusercontent.com/pw/AP1GczPWsn2C69JaMV4XBuINVD5T_x-HdfPJBFjPpiqOVcyAGbyMtUagzbjZmDUpPwIwZESgSEdrZDVUO-Yq_BrmQINuXZFplkjNI1DltOxl2b3uLbudCIWplKRgAdOG4kquf5vw1AF1peUmK7bGru6Kyr-V=w1157-h868-s-no-gm?authuser=2)

프로그램을 요약 해석하는 정적 분석기는 많은 오탐을 동반하게 된다. 그래서 규모가 큰 프로그램에서는 수천 개의 알람이 발생하는 것이 다반사이다. 이 연구에서는 과거 버그들에서 트레이스를 추출하고, 이와 비슷한 트레이스를 갖는 알람들에 우선 순위를 부여함으로써, 유사한 버그들의 탐지를 돕는 방법을 제시했다.
![](https://lh3.googleusercontent.com/pw/AP1GczOLq-e9-I-4UyPfoZUE5-P_z0jOCdDJunu4G0UfxSQTq4-W8c0kbxLj146XrO6YcjtFMsog1vDQl1hJbJozEHbCzUfeF5kD36R-IL9WYkk5i7t2EXMbKao5hC0rULnuavuoNWghsErtHvvCxEdHnms=w1157-h868-s-no-gm?authuser=2)

## USC 방문

학회 마지막 날인 금요일에는 교수님의 친구이신 Mukund Ragothaman 교수님을 만나고자 USC에 방문하였다. 약속 시간보다 일찍 도착하여 학교를 잠시 둘러볼 시간이 있었는데, 빨간 벽돌로 지어진 건물들이 인상적이었다.
![](https://lh3.googleusercontent.com/pw/AP1GczMnyq1WvLWKLZ8aV-XmkthkC_NAyRKxsHduoy9_FP94nA_-t3mSkqbDJuFYAvQ4WE4Q2oIFlY5wcujtinnHrL3Z7FHUuoj-FFVWL_jiPsUNOsdggadeTtPVAqknyqUa6jEwoyb6EWAZ9yNnv-SJyKo=w651-h868-s-no-gm?authuser=2)

USC에서의 일정은 Mukund 교수님이 잡아주셨다. 미국 대학의 문화인지는 모르겠으나, USC의 다른 교수님들과도 30분씩의 미팅 일정을 잡아주셨다. 그래서 Mukund 교수님을 포함하여 총 4 분의 교수님을 만나뵐 수 있었고, 현재 우리가 연구하는 내용 및 USC 교수님들이 연구하는 내용에 대해 이야기를 나눠볼 수 있었다.

## 마치며
연구실을 통해 좋은 기회로 CCS 및 USC를 방문할 수 있었다. CCS에 참석할 수 있도록 기회를 제공해주신 교수님과, 행정 지원을 해주신 행정실 직원 분들, 그리고 USC에 우릴 초대해주신 Mukund 교수님께 감사하다. 특히 USC에서 우릴 환대해주신 USC 교수님들의 따듯함은 지금도 기억에 남는다. 2월 달의 CAV 학회를 목표로 연구를 진행중인데, 잘 마무리하여 다음에는 내 논문을 가지고 학회에 방문할 수 있길 다짐한다.

[<a name="JitPicking">1</a>] Bernhard, Lukas, et al. "Jit-Picking: Differential Fuzzing of JavaScript Engines" CCS (2022) \
[<a name="NDI">2</a>] Qingyang, Qiushi, et al. "Non-Distinguishable Inconsistencies as a Deterministic Oracle for Detecting Security Bugs" CCS (2022) \
[<a name="DirtyCred">3</a>] Zhenpeng, Yuhang, Xinyu. "DirtyCred: Escalating Privilege in Linux Kernel" CCS (2022) \
[<a name="Tracer">4</a>] Wooseok, Byoungho, Kihong. "TRACER: Signature-based Static Analysis for Detecting Recurring Vulnerabilities" CCS (2022) \

