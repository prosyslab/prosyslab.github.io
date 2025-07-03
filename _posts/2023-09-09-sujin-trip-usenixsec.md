---
title:  2023 Usenix Security 를 다녀와서
date:   2023-09-09
author: Sujin Jang
kor_author: 장수진
tags:
  - Trip
  - USENIX Security 2023
classes: wide
---

# 들어가며
USENIX Security 2023이 8월 9일부터 11일까지 총 3일간 미국 Anaheim에서 열렸다. 같은 연구실의 태은님이 USENIX Security 2023에 논문이 채택되어서 함께 USENIX Security 학회에 참가할 기회를 얻게 되었다. 태은님 발표 응원겸, 최근 보안 분야에서는 어떤 연구들이 진행되고 있는지에 대해 경험할 수 있는 좋은 기회를 얻게 된 것이다.

<br/>

# 8/8 (Tue.)
모두가 좋은 상태로 학회에 참가할 수 있게 학회 시작보다 하루 일찍 미국에 도착하는 일정으로 출발했다. 처음 경험하는 12시간이라는 장시간 비행이 매우 걱정되었지만, 외부 전경이 꽤나 아름다워서 걱정했던 것에 비해 좋은 상태로 미국에 도착할 수 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczN7g4ikj631F-02uwDkZyR6NaY9eu3mctG4V76g7vs8LtAx4mzm7-Nl1vozxXz-ObdFajd7DjKq2-lCoervdvjcQoJc_lwy-ztH4NWHwYAwvW7gy0wLU1gsB_Brxbzx4fjOwfxccN42qeZN6QsuOSfw=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>구름위를 둥둥</b>|

| ![](https://lh3.googleusercontent.com/pw/AP1GczM5JgEH7CmmhPBYM3eXwqHjMLd5EzlixzHeJWitDEqrN2q2tkLkiqA4AcDUXxlk_srG_HHrwtPgFIYjf44oVT9X5X53OgIDkPjBQJf4s06XZSvS5FNR1b4eLFcUVUqEz_1tWyhPjyPkvDGjBgbx9lmF=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>하늘에서 본 노을</b>|

미국에 도착해서는 다들 장시간 비행으로 지쳐있었기 때문에 바로 호텔로 향했다. 호텔의 체크인 시간보다 이르게 도착하여 조금 걱정했으나, 호텔 프론트 직원분이 친절히 응대해주어 빠르게 숙소로 들어갈 수 있었다.

숙소에 들어가서는 잠시 정비 시간을 가진 후, 근처에 있는 디즈니랜드에 갔다. 마침 디즈니 100주년을 맞이하여 디즈니랜드가 화려하게 꾸며져 있었다. 입구에는 은색의 미키마우스 조형물이 설치되어 있었는데, 꽤나 귀여웠다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczM0pntEIDP31ed1Vgt5BFnSyA6jhulbSvjS32dvmjMY-IvjvWN9DOID7ttdDRHaGyRXGoKIr-YsNtI0kxbnkPDFOtSzowe8mppUo_V_juWtGALSTdQaln5FttnPpb355DcgQA7g8A5Gbau5pGynNI0K=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>100주년 미키마우스</b>|

저녁에는 교수님께서 미국에 계실 때 종종 가셨다는 **Ruth's Chris Steak House**에 갔다. 이제까지 먹어온 스테이크들과 비교도 안되게 너무나도 맛있어서 고기들이 사라져가는게 너무 아쉬웠다. 이곳에서 학회 참가 기간동안 처음이자 마지막으로 단체사진을 찍었는데, 직원분들이 고기가 잘 보이게 세팅도 도와주셨다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNxIO9eW1OPLeXequjC4LiBdsxDDQUBOWdSQfl5qMtakeAwJiJFYy6dDoZqCQSkHdJJfo8Eu-4VgU-PzAyTCwLRjZ2OZNpySg33xnhkqrg3PUWwmvxViihAJ_fqABaPcM_dDK2huNRrmIjog8S8TsoH=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>단체사진. 나름 고기도 강조된 사진</b>|

<br/>

| ![](https://lh3.googleusercontent.com/pw/AP1GczOq29zAjCDxKFBqWP1Qsi9-RuVLfUvQS95D_crcdQAuJIk6VrJoWQ-JlIv2h8phEdAkJnx3D_JTD3H4L72ZAd6nRu8Awo7yb1x3ylAz9yrEZaW8C4ztUbE69wnG_eRqmC-SAOdBe121UZninz4xdvWl=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>고기 확대 사진</b>|

<br/>

# 8/9 (Wed.)
드디어 학회 첫 날이 밝았다. 이번 USENIX Security는 매 타임마다 6개의 세션이 동시에 진행되었기 때문에, 궁금한 분야들이 동시에 다른 세션으로 진행될 수도 있어서 신중하게 세션룸에 들어가야 했다. 보안 학회이다보니, 내가 알고있는 것으로는 이해하기 어려운 내용들도 많아 알아듣지 못한 발표들이 많이 있었다. 이날 들었던 발표들 중 가장 인상 깊었던 발표를 공유하고자 한다.
<br/><br/>
**Towards a General Video-based Keystroke Inference Attack<sup>[1](#inference)</sup>**

입력하고 있는 자판 추론 공격 (Keystroke Inference Attack) 이란, 말 그대로 사용자가 입력하고 있는 자판이 무엇인지를 유추해내는 공격 기법이다. 이전까지 자판 추론 공격 기법이 많이 연구되어 왔으나, 대부분이 실제로 활용되기에는 어려운 가정을 많이 두고 연구되었다고 한다. 그래서 이 연구는 자판을 입력하고 있는 피해자를 녹화하고, 기계학습을 통해 영상을 학습하여 피해자가 입력한 자판을 추측하는 연구를 제안했다. 이 연구에서의 다음과 같은 가정이 필요하다.
- RGB 카메라, 예를 들면 핸드폰 카메라를 사용하여 자판을 입력하고 있는 피해자를 10분 정도 녹화할 수 있어야 한다.
- 영어만 입력해야 한다.
위와 같은 조건을 만족하면 녹화한 영상을 통해 피해자가 입력한 자판을 추측할 수 있게 된다. 자판 추측에는 기계학습을 사용하였으며, 강화학습을 통해 영상으로부터 자판을 학습한 후 DNN 모델을 통해 입력한 자판을 추측한다.
이 연구에서 배운 것은 '나쁜 마음만 먹으면 무엇이든 할 수 있겠구나.' 라는 것이었다. 누군가에 의해 몰래 촬영되고, 내가 입력한 자판까지 유추될 수 있다니 정말 무서운 세상이다라는 생각이 들었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNXgfdeghEpASeOvQKaMiJs44WCpwS_--eCW5-mH21TOtTjrQ_xaHytc55RloBeECnDFpjQDxUpTDBcT3KUGURqC4N-_wWl5XxGucOMnXfwBKf0bwEr9KqtpruCkgXbY5sMeuynwUg0ByXNQRuQe7wd=w1560-h699-s-no-gm?authuser=2) |
|:--:|
| <b>안전하려면 가리세요</b>|

<br/><br/>

# 8/10 (Thu.)
학회 둘째날이 되었다. 이날은 '곤충학 (Entomology)' 이라는 세션이 있었다. 이름이 흥미롭기도 하고, '소프트웨어 오류'들과 관련된 세션일 것 같아 해당 세션에 발표를 들으러 갔다. 확실히 이전 다른 세션들에 비해 관련이 있는 것 같다는 생각이 들긴 했지만, 여전히 발표들이 너무 어려웠다. 이 세션에서 들었던 발표들 중 가장 인상 깊었던 발표를 공유하고자 한다.
<br/><br/>
**Detecting API Post-Handling Bugs Using Code and Description in Patches<sup>[2](#post-handling)</sup>**

이 연구는 API의 사후 처리를 하지 않은 경우를 감지하는 방법에 대한 연구였다. API의 사후 처리란, API를 사용한 후, API의 반환 값을 확인하거나 자원 반환을 해야 한다는 사양을 의미한다. 이 연구에서는 이러한 API의 사후 처리가 누락되어 있는 경우를 탐지하고 오류를 보고하는 도구를 제안했다. 이 도구는 API의 사후 처리 누락을 탐지하기 위해 API 문서와 패치 정보로부터 필요한 사후 처리 정보를 추출한다.  
이 연구에서 배운 것은 '누구봐도 그럴듯한 가정에서 시작해야 한다.' 라는 것이었다. 처음 API를 작성하고 설계한 설계자는 해당 API가 어떻게 활용될 것이고, 사용한 후에 어떤 처리가 필요할지에 대한 정보를 사양 문서에 남겨두었을 것이다. 또한, API를 사용하는 개발자는 해당 API를 사용하면서 어떤 처리들이 필요하고, 오류가 났을 땐 어떻게 대처해야겠다와 같은 정보를 코드에 남겨두었을 것이다. 만약 잘못 처리했다면 패치 코드가 위의 내용을 담고 있을 것이다. 그래서 이 연구는 위와 같은 정보를 통해 API 사후 처리 오류를 탐지하는 도구를 개발하지 않았을까 싶다. 이 분야에 대해 잘 모르고, 이러한 연구가 진행되고 있다는 것을 처음 본 나도 '아 그래서 저런 정보를 사용했겠구나' 라는 생각이 들만큼 누가봐도 그럴듯한 가정에서 출발하여 연구를 진행하는 것이 필요하지 않을까라는 생각이 들었다.

그리고 이 학회에서 가장 듣고 싶었던 태은님 발표를 들으러 갔다. 항상 태은님 발표는 깔끔하고 전달력이 좋다고 생각했는데, 그 중에서도 단연코 가장 좋은 발표였다는 생각이 들었다.

**DAFL: Directed Grey-box Fuzzing guided by Data Dependency<sup>[3](#dafl)</sup>**

이 연구는 지향성 퍼징의 성능을 높이기 위해 대상 지점과 관련된 코드 부분들만 선별하여 퍼저에게 영향을 줄 수 있도록 하는 아이디어를 가지고 진행한 연구였다. 기존 지향성 퍼저들과 다른 방식의 피드백 점수 산정 방식을 제안하며, 기존 지향성 퍼저들보다 빠르게 오류를 재현하는 퍼저를 제시하였다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczN8OmdVd1omDMeC8Iex6satQQcF72OIN44t4K2BvQzC0Ot26pY_NZlp1Kh3FuQp7Lxxz4JZqiFA0pRdzdTx3UDhH6qCvlX2w4oH_k6mF8_m27-WCyJd-ZfJtZw9IFSZ2kpUW2XfX6UGTq7Myz3kcsQy=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>발표하는 태은님</b>|

두번째 날의 학회 일정이 끝나고, 저녁으로는 맥도날드의 빅맥을 먹었다. 한국에서도 먹어보지 않은 빅맥을 현지에 와서 처음 먹게 되었다. 연희님에게 감자튀김은 후추와 먹는게 맛있다는 정보를 듣고 바로 실천해서 햄버거와 맛있게 먹었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNL-DeDHLvG7XBGtR8zMNsexgQzq-DdAvwYU1VK4SppLn1O9vQbZvWFv6c4POPwMH7tNYXbCWLEhqAU8TLn06qdKSpsbPXSWiwhT0uiotOsKc7XffvdjqMZi70uTMVU_orKTHqBZSZ_-pllYKBkrAFD=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>후추가 뿌려진 감자튀김</b>|

<br/><br/>

# 8/11 (Fri.)
학회의 마지막 날, 이전까지 하지 못한 경험을 많이 한 날이었다. 학회 둘째날까지는 다른 사람들에게 말을 거는 것도, 대화를 하는 것도 너무 어렵고 쑥스러워서 대화에 잘 참여하지 못했었다. 그런데 셋째날이 되고 쉬는 시간에 세션룸 밖에 나와 앉아있으니 다른 분들이 와서 먼저 말을 걸어주어 서로 인사도 하고, 연구 이야기도 나눌 수 있었다. 직업을 찾고 있는 사람도, 직원을 구하고 있는 사람도 와서 말을 걸어주었다. 근데 아무래도 연구 분야가 보안 분야와는 거리가 멀다보니 서로의 연구 분야를 잘 이해하지 못해서 서로 멋지다는 말만 주고 받았다.
<br/>
학회가 끝나고 디즈니랜드에 방문했다. 화려한 퍼레이드와 불꽃놀이를 보러 방문했는데, 생각보다 시간이 남아 놀이기구도 몇 개 탔다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNeLZ1B9iDA54O2ykLsl4MTI8wqtZvfhEAWujac1ZaRj2038cZy0eR7P9bo6gd5JvVRv72PZxTO6bjfkkisTnu54ynt5yh0gioMU_344R8YilDsHPYQJ7wjvjVcxq-vXGwhkTh45U3eg5M8mkyd1tw1=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>고래 입으로 들어가서 디즈니 미니어처 구경</b>|

디즈니랜드에 가면 꼭 봐야하는 **디즈니 성** 앞에서 연희님이랑 사진도 찍었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczP_cB4v-BoAAk6R3MmKi1UzcShzZnSVxROm-sFIrHgfysuaehXO5OPAZhgsbEXJ7ZQZ2SQ9Nxu2DZ5b9qlWiXJZQq4JcRncUtv6GNJM6Z9a_DuEFFerGlypACnQ0CRr1DbS8l2Jbbc5ja0eQYWUfEI-=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>찰칵</b>|

퍼레이드가 6시 30분 시작이어서 자리를 잡고 15분간 이루어지는 퍼레이드를 구경했다. 시작하자마자 마음이 울렁울렁하더니 동심이 살아나는 것 같은 기분이 들었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPOeEg_SWNY1dUdZLh3i5fRGg_AtRQRW95evmbyqlacU3pbVd2fccm3mxLvUBed--zcL3HxO_z6YS9hm5B2VKAU46Nww2itWtWGsJ-g_PbAvJObs-DInLvCyvEvLaTSth6J1_YjlqP-KZhrMFbhRNkQ=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>모아나</b>|

이후에는 자유롭게 돌아다니다가 불꽃놀이 시작인 9시에 디즈니 성 앞에 자리를 잡았는데, 아쉽게도 바람때문에 불꽃놀이는 보지 못했다. 그래서 대신에 예쁜 디즈니 성의 야경 사진을 얻었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPQzI2EUDDeE_x4UVsjldleWQp-aZB3Azvviz1-3f9MBAZWvn5pbcsR-VVkvCw--G-J3HCGgmTA4weF7eHQf9mNADc4gN0ApRxqLLl7LwK2w8YdPceaC8709TOzbqOOahwAQxMKawbni-Redh06kgr4=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>디즈니 성</b>|

<br/><br/>

# 8/12 (Sat.)
한국으로 돌아가는 날, 산타모니카 해변과 게티 센터에 방문했다.
게티 센터에서 잔 폴 게티 (Jean Paul Getty) 가 소장하고 있던 그림과 조형물들, 그리고 아름다운 풍경을 구경할 수 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczMgqhUf3LiSf4ugdyxbl7PaVD_ABzWPH7ftw62v_paTCAqxD3dInGLB1YsqPuoOJCZ5YmuCazj-NZvx8h2B0IgA2LjlOXMh7MQf0v5H3LXnitopw7zCZggX51t1daGNvKIKwfbSnJRuodF1HFdFvsxD=w651-h868-s-no-gm?authuser=2) |
|:--:|
| <b>물이 졸졸</b>|

<br/>

| ![](https://lh3.googleusercontent.com/pw/AP1GczNuRb-d0Du4aVsrd_ntcO2HPurTPJ8ei36yKYMi0MLX_nUvFAS-dtXWoTSBu0z8ThLDXAD6F-8tD3PSKNrrDM6q7fokoNoM1ICNvnDBdCfnsO4cZBeAcub97RWkEoJsBy1S1sNgiq8C2a5nIjaIYDSi=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>강아지 모양 구름</b>|

그리고 산타모니카 해변에서는 일몰을 볼 수 있었는데, 저녁하늘이 이렇게나 아름다웠다는 것을 새삼스럽게 느낄 수 있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPLnFS98BW85do548Faj1UCnYWxoJYY6sfvVYOPChOFHv4A5iENDc1HMREWUhhpk5d0f8bsFpymwiSUKqHP_TpLJKXtM6TAiOZqP6GsamjwIZtSDxY3lBT-xC5ciAlgxYyfme2naBcfnoW0gJf9C00i=w1157-h868-s-no-gm?authuser=2) |
|:--:|
| <b>산타모니카 해변의 일몰</b>|

<br/><br/>

# 마치며
연구실을 통해 USENIX Security 라는 좋은 학회에 방문할 수 있었다. USENIX Security에 참석할 수 있도록 기회를 제공해주신 교수님과 좋은 논문 발표 해주신 태은님, 함께 학회를 즐기며 좋은 구경할 수 있게 해준 연희님과 종찬님, 마지막으로 출장 준비를 도와주신 나은진 선생님께 감사드린다. 마지막으로 현재 준비하고 있는 논문 잘 마무리해서 다음에는 내 논문을 가지고 학회에 방문할 수 있기를 바란다.
<br/><br/>

----


### 참조
[<a name="inference">1</a>] Zhuolin Yang et al., "Towards a General Video-based Keystroke Inference Attack", USENIX Security (2023) \
[<a name="post-handling">2</a>] Miaoqian Lin et al., "Detecting API Post-Handling Bugs Using Code and Description in Patches", USENIX Security (2023) \
[<a name="dafl">3</a>] Tae Eun Kim et al., "DAFL: Directed Grey-box Fuzzing guided by Data Dependency", USENIX Security (2023)
