---
title:  두 번 가서 배로 좋은 PLDI와 FSE 여행기
date:   2025-07-28
author: Sujin Jang
kor_author: 장수진
tags:
  - Trip
  - PLDI2025
  - FSE2025
classes: wide
---

# 들어가며
PL 분야의 큰 학회인 PLDI가 6월 16일부터 20일까지, SE 분야의 큰 학회인 FSE가 6월 23일부터 25일까지 각각 서울과 노르웨이 Trondheim 에서 열렸다.

같은 연구실의 봉준님의 논문이 PLDI 2025에 채택되어 기쁜 마음으로 응원가는 겸, PLDI SRC 2025에 제출했던 내 논문도 채택되어 포스터 발표를 하기 위해 PLDI에 참석하였다.
그리고 연희님, 그리고 지금은 군대를 가신 희원님과 열심히 작성했던 논문이 FSE 2025에 채택되어 학회에 참석하게 되었다.

<br/>

# 6/16 (Mon.)
PLDI의 주요 발표들은 수요일부터 이루어졌지만, 교수님의 전폭적인 지원으로 워크샵부터 참여할 수 있는 기회가 주어졌다.
아침 5시 반부터 이동하며 약간 피곤함을 느꼈지만, 최신 프로그램 분석 분야의 논문 발표를 들으면서 학회에 왔다는 것을 실감하기 시작했다.

그리고 맛있는 점심 도시락은 잠을 확실하게 깨워주었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczM4uZ2boNfNROOOtOCD7nUhyPUxtq69rvQVCu1N2EpXTV5RIT2N52-wd3_zfP-59hRZD2Q62_Frkad4Nsk_F2C_7eTd507Y0oFBpjnB_-BnpMW0KehO19_pfBGczg3-xD5pM_sTznCp_jPHD_DuxYDK=w1230-h923-s-no-gm?authuser=0) |
|:--:|
| <b>비싸고 맛있는 도시락</b> |

<br/>

오후 2시부터는 PLMW라는 학생 연구자들을 위한 친목(?) 활동과 교수님들의 다양한 조언을 들을 수 있는 워크샵에 참석하였다.
친목 활동 중 하나로는 관심 분야의 사람들끼리 조를 짜고 대화하는 활동이 있었는데, 프로그램 합성 분야는 학생 연구자들의 관심이 많이 줄은 것인지 조가 따로 만들어지지 않았다.
그래서 방황하다 타입 시스템 분야에 가서 사람들과 이야기를 나누었다.
간단한 자기소개를 하면서 이야기를 시작했는데, 내가 명찰에 대학원생이라고만 적어두었더니 석사인지 박사인지를 다들 궁금해했다.
그래서 다음부턴 학위 과정을 명확히 써야겠다는 생각이 들었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczMIlJKnBtl_IIHB_7klN0XKnLP_WveyMaX99UuSCJVa7NeIU7TgswrNKiLmnrh_Cy43soVoGMpTtP8ZUJJZlZydAwPItFijCRw7HEyeHasxEsFTEf15YwU5SzwAUyFsmfamkQ6XSLquKYV-q-luqTZa=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>다음부턴 박사과정이라고 적자!</b> |

<br/>

다들 왜 이 조로 왔는지를 이야기 했고, 나는 다른 연구를 하는데 배우고 싶어서 왔다고 이야기 했더니 내 연구에 대해 더 궁금해하여 설명하게 되었다.
그리고 결국 타입 시스템 연구에 대해서는 많이 듣지 못한 채 세션 시간이 끝나 나오게 되었다.
그래도 수요일에 포스터 발표를 한다고 홍보도 하였고, 그때 자리에 함께 있었던 한분이 실제로 포스터를 구경 오시기도 하였다. :>

<br/>

# 6/17 (Tue.)
교수님들의 강연으로 PLMW 세션이 가득 채워져있었고, 하루 종일 발표를 들었다.
교수님들은 대학원생 때부터 현재까지 학계에 있으면서 겪은 다양한 경험들을 공유해주셨고, 필드에서 쓰일 수 있는 연구를 하는 게 중요하다는 것을 거듭 강조하셨다.
제안서를 쓸 때도 중요하지만, 회사에 기술을 넘기는 것까지 많은 교수님들이 생각하고 계신 것 같았다.
"지치지 않고 문제를 찾는 것, 그리고 그 문제를 잘 푸는 것" 말은 너무 쉽지만 실행하기는 쉽지 않은게 인생과 참 비슷하다는 생각이 들었다.
어쩌면 연구는 인생을 더 잘 살아가는 방법을 찾는 과정을 배우는 것인지도 모르겠다는 생각도 들었다.

저녁에는 리셉션이 있었고, 비어있는 테이블이 있어 신나하며 자리를 잡았더니 많은(?) 사람들이 인사를 하며 대화를 하러 왔었다.
한번은 교수님과 같이 프로그램 분석 분야 연구의 미래에 대해 이야기를 하고 있었는데, Yizhou Zhang 교수님이 다가오셨다.
Zhang 교수님은 당일 PLMW 에서 발표를 하셨어서 기억하고 있었고, 발표를 들었다는 것을 어필하며 내 연구에 대해서도 간단하게 설명드릴 수 있었다.
간단한 연구 설명만을 준비했어서 조금만 더 궁금해해도 설명하기가 조금 어려웠는데, 여러 번 반복하다보니 더 나중에 만난 사람들에게는 더 잘 설명할 수 있게 된 것 같았다.  

| ![](https://lh3.googleusercontent.com/pw/AP1GczP750uzDEWPMe9l-fXnbDOMpcpaoA9-wytFMh9N_6Y41xOroMca-fxDmKmqjrPqotXoGYV5kaIdYVTL6ro0o5x7eWxta9muDGGetHHZrnzGz9YoeY_Ey1VAW5_9fjQG_rblBAvIyUT48RlB6VbGGjGf=w1230-h923-s-no-gm?authuser=0) |
|:--:|
| <b>일정 끝난 후 학회 인증 사진</b> |

<br/><br/>

# 6/18 (Wed.)
류석영 교수님의 멋진 기조 연설을 시작으로 PLDI의 주요 일정이 시작되었다.
첫 날에는 이 넓은 공간이 가득 채워질 수 있다고? 싶었던 호텔의 그랜드 볼룸이 가득 차고, 의자가 부족해 바닥에 앉아서 연설을 듣는 사람들도 있었다.
이런 멋진 공간에 함께 있을 수 있음에 뭔가 벅차오르는 감정이 들었다.

이 날은 PLDI에서 드물게 볼 수 있었던 프로그램 합성 세션이 있는 날이었다.
PL 분야니까 합성 연구가 좀 많지 않을까? 라고 기대했던 학회 전과 다르게, 합성 연구 논문이 많지 않아서 조금 아쉬웠다.

합성 연구 중 가장 기억에 남는 연구는 2편이 있었다.
한 편은 SyGus 에서 성능을 끌어올리기 위한 연구<sup>[1](#synthesis1)</sup>였는데, 테스트 케이스를 잘 가르는 분기문을 찾고자 하는 연구였다.
Duet<sup>[2](#duet)</sup>이라는 굉장히 잘하는 도구가 있어서 이보다 더 잘할 수 있나? 하는 궁금증이 있었는데, 더 잘할 수 있는 방법이 있다는 것이 놀라웠다.
UnitCon도 다른 사람들이 보기에 이렇게 보이려나 싶긴 했다.

다른 한 편은 반복문 실행 횟수를 정확하게 계산하는 연구<sup>[3](#synthesis2)</sup>였다.
반복문이 종료했을 때 값이 0이 되는 카운터 변수를 두고, 초기 카운터 변수를 계산하는 함수를 합성하는 것을 목표로 하는 연구였다.
실행 횟수의 상한이나 하한 중 하나만을 굉장히 안전하게 계산하던 다른 연구들과 다르게 정확한 실행 횟수를 찾으려고 한다는 점이 더 발전한 연구라는 생각이 들었다.
그리고 특히 카운터 변수를 두어 종료 시점에 항상 0이 되도록 한다는 간단한 조건을 만족하는 함수를 찾는다는 아이디어가 좋다는 생각이 들었다.

저녁 시간에는 PLDI SRC 포스터 발표 시간이 있었다.
포스터를 설치하고 시작 시간이 되자마자 굉장히 많은 사람들이 내 포스터에 관심을 가져주었다.
심사위원 분들이 4분 정도 왔다 가셨고, 많은 학생들과 교수님들이 내 연구에 관심을 가지고 공감해주어 기쁜 시간을 보낼 수 있었다.
설명을 하면서 그 순간에도 연습이 되었는지, 시간이 갈수록 말이 조금 더 쉬워지는 느낌이 들었다.
부족한 영어에도 끝까지 포스터를 이해하려고 노력해준 학생들과 교수님들께 감사드린다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczO02DNwkyS761CaMB6fWc2d7f2LUu0ytTn1wDdqOD5973Kj7T0ZHqTrj_0ONbEMKqlIEcJ6wocJ8-95lXrKB_RSZG9C2seiPWL0oZe5TMq-Po_Oyr0WJQ_6u4lpMiE82FyixxcMFlrHXT03Ool0P3kZYg=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>유닛콘 스티커를 주고 싶어 파우치를 꼭 손에 쥔 나</b> |

<br/>

참고로 다른 학회에서도 주는지는 모르겠지만, PLDI SRC는 인증서도 준다.
멀리서 보면 상같기도 해서 기분이 좋다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczMnZRuP9QCeH1BWvAysZXXTykpoEBta40_E_NTX9KMghTA-TZRw2XEIxaO1LUurtjH6gL2S8Cw9kjyeMJxg52D7VVq-AY9bdEJToy_FRrA-9gOKhxdsog51B78XdCcHobgDH3M0G9PennwyZmlTAiUb=w713-h923-s-no-gm?authuser=0) |
|:--:|
| <b>SRC 참가자 인증서</b> | 

<br/><br/>

# 6/19 (Thu.)
학회를 마무리 하며 비즈니스 미팅이 이루어졌었다.
홈 그라운드에서 열린만큼 많은 한국인들이 학회에 참여했었고, 허충길 교수님께서 연산자 오버로딩같은 개념으로 한글을 설명할 때는 다 같이 웃기도 했다.

저녁에는 다양한 상의 수상자들을 축하하며 코스 요리가 제공되었는데, 정말 너무 맛있었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczN0nGwANTigUAWRqof8FtKTfV1921_gIHfwF_BvZQtMGDT-yCy3kdzYUIJMdtC9O_G3pyoVTonNCNYGc2B54ISLerrWXEit5HIK4i43NDuFpzG6o3TS7H0jdxTKCfqAmkIo3pjyrCADpjTSxWMqS_Ub=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>보기도 좋은 맛있는 고기</b>|

<br/><br/>

# 6/20 (Fri.)
PLDI 학회의 마지막 날이었다.
오전 키노트에서는 Işıl Dillig 교수님이 뉴로 심볼릭 연구에 대한 이야기를 해주셨다.
각 목표에 맞는 DSL (Domain-Specific Language) 를 정의하여 프로그램을 합성하는데, 구체적인 내용을 LLM으로부터 알아오는 연구들이었다.
예를 들어 이미지 수정을 목표로 하는 연구에서는 이미지 수정에 맞게 객체 찾기, 블러처리 하기 등의 동작을 정의한 DSL이 있고, 각 객체를 LLM으로부터 알아오도록 구성이 되어 있었다.
여전히 LLM이 이상한 답을 주면 올바른 프로그램을 못 만든다는 한계가 존재하긴 했지만, LLM을 활용한 연구의 성공적인 사례가 아닐까 생각이 들었다. 

| ![](https://lh3.googleusercontent.com/pw/AP1GczPwQsBX8893ej1-SVkGLPbbAzUPTAYfBpwiyoITFh16CvLqF4lq4eygUwVKVen-llvg5APpzzY2UCv7rq9IuAoPeG9ve_isYj_4vrPcJZjsUU0AwSvMEal4EdpB1oRe_cE0jCebhkOYqECP2ktpn9D4=w691-h923-s-no-gm?authuser=0) |
|:--:|
| <b>이미지 수정에 사용된 예시</b> |

<br/>

봉준님은 학회의 마지막 날 [Optimuzz](https://prosys.kaist.ac.kr/optimuzz/) 발표를 하셨다.
긴장한 티가 하나도 나지 않으면서 발표를 엄청 잘 하셨는데, 그 모습이 너무 대단하게 느껴졌다.

점심식사 후 월요일에 PLMW에서 만났던 애플에 다니시는 분을 만나 이야기를 나눌 수 있었다.
애플에서는 C에서 Swift로 넘어가려는 작업이 많이 진행되고 있다는 이야기를 들었다.
그리고 실제 기업 입장에서는 오버헤드를 절대 무시할 수 없어 비용을 최소한으로 줄이면서 근본적인 문제를 해결하는 방안에 대해 계속해서 연구하고 고민하고 있다는 이야기도 들었다.
연구자가 보는 작은 오버헤드와 기업 입장에서 보는 작은 오버헤드에는 차이가 있을 수도 있겠다는 생각이 들었는데, 자리를 뜨고 든 생각이어서 질문하지는 못했다.
명함도 받았는데, 근래 본 명함 중 가장 예쁜 명함이라는 생각이 들었다 :>

<br/>

# PLDI가 끝나고 FSE 시작 전
노르웨이로 가기 위해 재정비 시간이 필요했다.
그래서 금요일 오후에 학회가 끝난 후 대전으로 내려와 짐을 새로 싸고, 토요일 오후에 비행기를 타러 인천으로 갔다.
노르웨이를 가기 전 무엇을 먹어야 가장 좋을까 고민하다가 떡볶이를 먹었는데, 조금 아쉬웠던 것 같다. 돌아오면 다시 떡볶이를 먹기로 하고 비행기에 몸을 실었다. 

<br/>

# 6/22 (Sun.)
노르웨이에 도착한 이 날은 학회 기간 동안 유일하게 맑은 하루였다.
기온은 20도 안팍으로 한국과 다르게 시원했고, 바닷가 근처여서 그런지 바람은 더 시원했다.
체크인 전까지 시간이 남아 관광을 가기로 했다.
근처에 Munkholmen 이라는 감옥, 수도원, 요새로 그 용도가 계속 변화한 역사가 있는 섬을 방문하였다.
페리를 타고 이동할 수 있었는데, 운행 시간이 정해져있어서 기다리면서 아이스크림도 먹고 마지막 바이킹 동상도 구경했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNIoeR5JvUoRAJSlYy0z4kQhjQS7hK2k-pbogxgFfTRLpSwCFplxYSf0EtqmRZtbtklrTNFVuEUlUoB2jO6wtITqKfK2E7kh9hwLhf-yYNIveI4j5mSVycH161BoBVdtV3xckbjvaZKdtPQxUWC0fj4=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>마지막 바이킹</b> |

<br/>

| ![](https://lh3.googleusercontent.com/pw/AP1GczNm2XDO_2IrTRaLt9xrssh1kmVTr6FoUgjlA0VCYL0-WUF02buo5YOVJJAAIcJ8Y4QF12DazGUT7rUjacqQEOzmL1JDHk3ufv25AYe8_udJAp81Um6OBkj4_-9oBrZf-5oSVGbD0dDfQqr27dcemnM0=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>춥지만 아이스크림은 못 참아!</b> |

<br/>

섬으로 이동해서는 섬의 역사에 대한 설명을 간단하게 듣고 각자 돌아다니는 시간을 가졌다.
어떻게 섬 하나가 감옥, 수도원, 요새로 쓰일 수 있지 하는 의문이 들었는데, 직접 둘러보고 나서는 쓰일만한가? 라는 생각이 자동으로 들게 되었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPn4-9Rlh0zbz5OoL_a-0Ye1Z6fpB2TMMH9Mdo4f1zCdkrrwQ7FFsF6iIj_akFLMuVG3rr54-d_ms-juDU-7pa4Rzv0NFhqYGsFIu3PEmS12U-GYph2UHzHIb5alhEjJPSfzYvyIxQ8-n6kjZDv6TD7=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>공기 좋고 맑은 Munkholmen에서</b> |

<br/>

# 6/23 (Mon.)
학회의 첫 날이 밝았다.
[UnitCon](https://prosys.kaist.ac.kr/unitcon/) 발표가 첫 날에 있어 너무 긴장한 상태로 하루를 보냈다.
발표 전 청심환도 챙겨먹고 발표장에 갔는데, 예상치 못한 일이 너무 많이 일어나서 당황스러웠다.
발표자료를 넘길 리모컨이 따로 주어지지 않았고, 노트북이 있는 단상은 나에게 너무 높았다.
발표 전 공용 노트북이 잠겨 발표 시간에 촉박함을 느끼기도 했다.
이래저래 당황스러움을 느꼈던 나는 그게 발표에서 다 드러나게 되었다.
아쉬움이 많이 남았었기 때문에 빠른 재도전을 해야겠다는 생각이 들었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczM-iPIBsADRm1S9Qz8ONsdITH5w9ZrpLHDJuDU6uJzWMhWIQjhtyi_GHsu0xCXTAXov8MfaqLdj9vb4hie8y06NzxsMnl3z_pevhxfuRmkdn_VonSHeZfHsVce4cdwPj2cIdPLCJ3mvJ7z5OhupAzWG2Q=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>팔이 걸쳐진 이유는 너무 높아서 입니다.</b> |

<br/>

발표가 끝난 후에는 소문으로만 들었던 따뜻한(?) SE 학회답게 관광을 다 같이 갔다.
트론하임에는 니다로스 대성당이 있는데, 이곳에서 오르간 연주를 보여준다고 하여 성당으로 갔다.
중세 느낌이 물씬 느껴지는 오래된 건물이었다.
웅장했고, 정교했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczNX5BrWhY7WdPVf2zvNtwjZn7prNDaKBuGTIs4rITnuPmqBB59pKO3MzTq3TqXG2cnVmuaI_hrAgJdhTT6VHhnMzK8h1WP5pW9rXPe4yW6osrtiM9EJ0BaCQOs0dPlQXXGtj77n4_0XeY0zn3uOwcfm=w1230-h923-s-no-gm?authuser=0) |
|:--:|
| <b>니다로스 대성당</b> |

<br/>

그리고 어쩌다보니 백야(?) 기간에 북유럽에 방문하게 되어 하루종일 어둡지 않은 하늘을 볼 수 있었다.
밤 11시에 해가 지고 새벽 3시에 해가 뜬다고 했는데, 백야가 맞는지 아닌지는 정확히 모르겠다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczO2yBrTppgvER-W3qchfjCodI9mBMvOGANSB-J-nsklLoxxq_KPFEtR2KlFdR9sAQ6-RFwHe7kizVZelisdr30FNMNpncPDi6lECcwwENh_CaNiZETXtI4NR3s8Kjvo3ohjOJKB-Qjah67vxUeCDehN=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>이 하늘이 밤 12시라니!</b> |

<br/><br/>

# 6/24 (Tue.)
발표를 끝냈기 때문에 이 날부터는 편한 마음으로 발표를 열심히 들으러 다닐 수 있었다.
분야가 굉장히 다양했고, 리서치 트랙의 논문 뿐 아니라 저널, 인더스트리 논문들이 분야별로 묶여 발표가 진행되어서 발표 시간이 각양각색이었다.
그래서 그런지 교수님들의 발표도 제법 많이 볼 수 있었다.

테스팅은 확실히 인기 있는 분야인지 세션이 4번이나 열렸다.
이 날은 3번째 테스팅 세션이 있었는데, COBOL 테스팅을 자바로 옮기는 연구<sup>[4](#testing1)</sup>와 여러 종류의 테스트 오라클을 한번에 보여줌으로써 디버깅을 용이하게 하는 연구<sup>[5](#testing2)</sup> 등에 대한 발표를 들을 수 있었다.
같은 테스팅 분야에 묶여있었지만, 각 발표가 모두 특색있었다.

저녁에는 뱅큇이 있었고, 각종 상의 수상을 축하하며 코스 요리가 제공되었다.
UnitCon은 우수 논문상을 받아서 많은 사람들의 축하를 받을 수 있었다.
어떤 논문이 우수 논문상을 받는지 기준도 궁금했었는데, 리뷰 점수의 평균이 3.67점 이상인 논문들 중에서 골라진다고 하는 것 같았다.
이때 리비전 후 점수가 변경되었으면 변경된 점수로 계산한다고 했다.
논문을 열심히 쓰고 리비전도 열심히 했더니 좋은 결과가 있었던 것 같다. 

| ![](https://lh3.googleusercontent.com/pw/AP1GczNcK8s8X1ZYzAxLbjcFkNu3tKuaFMuBSkj8AIwd_c5cHg0jCiZkcejyNDRWh5m1WYfIQQ7vVggnuxeK30OcaMvKGNJSIeJRMf0QOBWIJsbe4TvILMIN9vlkTdbrNrGVcOOaVm3dGVjIdlU--LYU__OKUw=w1230-h923-s-no-gm?authuser=0) |
|:--:|
| <b>3팀씩 사진을 찍었다.</b> |

<br/><br/>

# 6/25 (Wed.)
FSE 일정이 끝나면서 ISSTA가 시작되는 날이었다.
새로 등록하는 사람들이 많아지면서 다시 학회장이 북적북적해졌다.
이날도 어김없이 테스팅 세션을 찾아 다녔다.
연산 리소스 관련된 flaky test에 대한 조사 논문<sup>[6](#testing3)</sup>에 대한 발표, 가짜 객체 (mock)을 사용하는 테스트의 특성을 조사한 논문<sup>[7](#testing4)</sup>에 대한 발표를 들었다.
가장 기억에 남는 것은 0.5CPU와 2GiB RAM을 사용하면 연산 리소스의 flaky test를 피할 수 있다는 것이었다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczP6F1sbPQf2ypRWhFG33CFJ3WIahFgP82QVfLAMN4cEz8xHMgmG7RJuZM3CDmMMST7o9nnOxd_-9h6-Rl5PcuvsIw1EcusG6haterrPCWNVfXdlmfntbn8aczkL8WjwNr5qZeG3piDFU-WzhetK1wBI=w1230-h923-s-no-gm?authuser=0) |
|:--:|
| <b>연산 리소스의 flaky test를 피하기 위해 참고하자</b> |

<br/>

점심은 파스타와 샐러드 등을 자유롭게 가져가 먹을 수 있게 제공되고 있었다.
그래서 자리에 앉아 음식을 먹는데 충북대의 기은님과 Stuttgart 대학의 Beatriz Souza가 와서 같이 대화를 하며 밥을 먹었다.
Beatriz Souza가 링크드인을 보여주었는데 팔로워가 엄청 많아서 신기해했더니 웃긴 사람들이라며 엄청 웃었다.
FSE에서도 꼭 스티커를 나눠줘야지 라는 생각으로 PLDI에 챙겨갔던 파우치를 들고 갔는데 드디어 한 개를 나눠줄 수 있었다.
나름 성공적(?)인 교류였다는 생각이 들었다.

FSE 학회 일정이 끝나고는 근처에서 하는 플리마켓 행사를 구경가기 위해 나왔다.
버거 패티 냄새가 유혹했지만, 잘 참고 구경을 다녔다.
밴드 공연도 구경하고, 다양한 상품과 음식들도 구경했다.
그 중 가장 기억에 남는 것은 많은 종류의 치즈가 진열된 곳이었는데, 치즈 종류가 너무 다양해서 신기했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczO-F3C8PDGZm4glFo9t9ohv6bqtWimsl6qzlET9gfxQ9vb8kQ892tkLmAOgXOue7Ii4mUxrbXtMP3xsWAJY94AxW3XcwbGY9hbq9pyjVv-Nw_8eSA84rRcemansFd7H4PzLorjIJt3UlVpcp5sQq3OJ=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>녹색 치즈가 신기합니다.</b> |

<br/>

새로운 도시를 가니, 익숙했던 서울과 다르게 낯선 느낌이 여행에 재미를 불어넣어준 것 같았다. 

<br/>

# 6/27 (Thu.)
한국으로 돌아가는 날이었다.
오전에는 전날 3배 정도 비싸게 주고 구매한 노르웨이 바세린을 환불하러 다녀왔다.
한국에서도 환불을 잘 하지 않는 편인데, 왠지 지금이 아니면 절대 환불을 할 수 없다는 생각 때문인지 용기가 나서 무사히 환불을 잘 하고 나왔다.
다들 가격 비교를 잘 하고 사자!

| ![](https://lh3.googleusercontent.com/pw/AP1GczNATzqG-O1O2ZSx0a1focHPiCAqbcJOOdkyOfoMYRt1milaM9dS19vF86-JsrvQRxkcLmloYgslvga_EotHbJtE8LlMt8G7uiUjH5OHtaxm_S8LMeqyf9QBBRD3k7nBdB_DuOHMOurAqyvCKb_AN4MP=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>약국에선 69 크로네, 여기선 24 크로네!</b> |

10시 반에 체크아웃을 하고 교수님, 연희님과는 각자의 시간을 보내다가 점심에 학회장에서 다시 만나기로 하고 흩어졌다.
나는 카페에서 커피를 마시며 조금 쉬기로 하였다.
코르타도 라는 스페인식 카페라떼를 시켜 마셨다.
한국에서는 무조건 아이스 아메리카노를 시켜먹는 나로썬 새로운 도전이었다.
씁쓸하고 부드러운 게 꽤 먹을만했다.

| ![](https://lh3.googleusercontent.com/pw/AP1GczPbF9XumQrN3NfUuT7Kuiu2Ue2lUUWV1KFvC1gCbLIEtIOC-69QYVYgVNvUjL8jS9MyNJn0qoIMiTnNmk0BdhsB21FMBcpySk3yTRrXqv3s6MCMjYmF8vBGCxkCMUmElR9LUA4mOMF5NMt3v68RyR5-=w693-h923-s-no-gm?authuser=0) |
|:--:|
| <b>나름 아트도 있다.</b> |

<br/><br/>

# 마치며
교수님의 전폭적인 지원과 좋은 기회로 큰 국제 학회 두 곳에 참석할 수 있었다.
다양한 연구자들을 만나고, 연구에 대한 열정을 느낄 수 있어서 배운 점이 많았던 일정이었다는 생각이 들었다.
좋은 논문 발표를 해주신 봉준님, 함께 PLDI부터 FSE까지 긴 여정을 함께 해주신 연희님, 마지막으로 출장 준비를 도와주신 김은주 선생님께 감사드린다.
2년 전 내 논문을 가지고 학회에 방문하고 싶다는 꿈을 이루게 되어 기쁘다.
지금 연구도 잘 마무리하여 내 논문을 가지고 다시 학회에 방문하고 싶다.
<br/><br/>

----

### 참조
[<a name="synthesis1">1</a>] Yuantian Ding and Xiaokang Qiu, "A Concurrent Approach to String Transformation Synthesis", PLDI (2025) \
[<a name="duet">2</a>] Woosuk Lee, "Combining the Top-down Propagation and Bottom-up Enumeration for Inductive Program Synthesis", POPL (2021) \
[<a name="synthesis2">3</a>] Daniel Riley and Grigory Fedyukovich, "Exact Loop Bound Analysis", PLDI (2025) \
[<a name="testing1">4</a>] Sandeep Hans et al., "Automated Testing of COBOL to Java Transformation", FSE Industry (2025) \
[<a name="testing2">5</a>] Matthew C. Davis et al., "TerzoN: Human-in-the-Loop Software Testing with a Composite Oracle", FSE (2025) \
[<a name="testing3">6</a>] Denini Silva et al., "The Effects of Computational Resources on Flaky Tests", TSE (2025) \
[<a name="testing4">7</a>] Hengcheng Zhu et al., "Understanding and Characterizing Mock Assertions in Unit Tests", FSE (2025) 
