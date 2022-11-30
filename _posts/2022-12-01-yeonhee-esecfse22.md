---
title:  ESEC/FSE 2022 @ 싱가포르
date:   2022-12-01
author: Yeonhee Ryou
kor_author: 류연희
tags:
  - Trip
  - ESEC/FSE'22
---

코로나 이후 3년만에 오프라인에서도 ESEC/FSE 학회가 열렸다. 교수님과 다른 학생들이 참석한 CCS 바로
다음주에 진행되는 일정이어서 ESEC/FSE 는 혼자 참석하게 되었다. 학회가 열린 싱가포르는 11월에도 덥고
습했다. 혼자여서 좋았던 점도 있었고 아쉬웠던 점도 있었지만 많이 배울수 있는 기회였다.

## 개회식과 기조 발표

개회식에는 다양한 통계가 발표된다. 코로나 시즌에 온라인 학회를 들으면서 분야의 연구 동향을
파악하려면 개회식을 잘 들어야한다는 것을 알게되었다. 그 중에서도 분야별로 제출된 논문과 승인된
논문의 통계를 본다.

이번 ESEC/FSE 에도 가장 많이 발표된 주제는 "AI and ML for SE" 분야였다. 학회 전체적으로 논문 총
469편이 제출되었고 99편이 승인되었는데, 그 중 "AI and ML for SE" 분야에 제출된 논문은 125편이고
승인된 논문도 36편이라고 한다. 전체의 1/3 이나 되는 것이다. "Software testing" 이 세번째, "Program
analysis" 가 다섯번째로 제출 편수가 많았는데 비해, 승인된 논문 수는 둘을 합쳐도 "AI and ML for SE"
분야보다 작았다. 두가지 모두 오래된 분야인 만큼 상대적으로 새롭고 중요한 연구가 나오기는 어려울 수
있지만, 다소 치우쳐 있다는 인상을 받았다.

개회식 이후에는 바로 Sumit Gulwani의 기조 발표가 이어졌다. 이번에 학회에 참석하면서 가장 기대했던
발표였다. 제목은 "AI-assisted Programming" 인데, 프로그램 합성에 사용되는 다양한 기술을 포괄적으로
다뤘다. 프로그램을 합성하기 위해서 프로그래머의 의도를 알아낼 수 있어야하는데, 이 발표에서는 (1)
입출력 예제, (2) 자연어, (3) 현재 작성 중인 코드의 맥락(Temporal context), (4) 수정 이력을 이용해서
프로그래머의 의도를 기술하거나 유추하는 방법을 다뤘다. 입출력 예제 기반의 귀납적 프로그램 합성
(Inductive synthesis) 기술에서 출발해서 GPT-3와 Copilot을 비롯한 최신 언어모델 기술, 그리고 이들을
융합하는 다양한 방법까지 폭넓게 다루어서 참고가 되었다.

기조 발표 역시 AI (and ML) for SE 를 주제로 한 셈이다. 2박 3일 학회 일정 동안 유일하게 기계 학습
분야만 세개 세션으로 진행될 정도로 발표 논문이 많았다. 이 외에도 다른 세션에서 발표된 인공지능과
기계 학습 관련 기술을 포함하면 절반 이상이 해당될 것 같다. 소프트웨어 엔지니어링 분야에 인공지능과
기계 학습이 적용된지도 오래되었다. 이제는 좀 더 연구 주제를 세분화하고 구체적인 문제를 다룰 수
있어야할것 같다.


## 심층 학습, 그 중에서도 트랜스포머

기계 학습 중에서도 심층 학습, 그 중에서도 트랜스포머를 사용한 연구가 많이 보였다. 내가 지금
사용하는 도구여서 더 눈에 잘 띄었을지도 모르겠다. 가장 두드러졌던 것은 Program Repair/Synthesis
세션이었다. 총 5편의 논문 중에 오학주 교수님 연구실 학생이 발표한 PyTER[^1] 논문을 제외하면 네 편이
모두 트랜스포머 언어모델을 사용한 논문이었다. 그 중에서도 두 편[^2][^3] 이
[CodeT5](https://github.com/salesforce/CodeT5) 를 이용했고, 한 편[^4]은
[CodeBERT](https://github.com/microsoft/CodeBERT) 를 이용했으며, 단 한 편[^5] 만 자체적으로
[BART](https://arxiv.org/abs/1910.13461) 기반의 모델을 사전학습하여 사용했다.
BART 를 사용한 팀이 Microsoft 의 연구팀이기 때문에 네 편의 논문 모두 대기업이 사전 학습한
[프로그래밍 언어 모델](https://github.com/prosyslab/pl-wiki/wiki/%EC%BD%94%EB%93%9C-%EC%96%B8%EC%96%B4-%EB%AA%A8%EB%8D%B8)
을 사용한 셈이다.

[^1]: Wonseok Oh and Hakjoo Oh. 2022. *PyTER: effective program repair for Python type errors.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 922–934. [https://doi.org/10.1145/3540250.3549130](https://doi.org/10.1145/3540250.3549130)

[^2]: Michael Fu, Chakkrit Tantithamthavorn, Trung Le, Van Nguyen, and Dinh Phung. 2022. *VulRepair: a T5-based automated software vulnerability repair.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 935–947. [https://doi.org/10.1145/3540250.3549098](https://doi.org/10.1145/3540250.3549098)

[^3]: Misoo Kim, Youngkyoung Kim, Hohyeon Jeong, Jinseok Heo, Sungoh Kim, Hyunhee Chung, and Eunseok Lee. 2022. *An empirical study of deep transfer learning-based program repair for Kotlin projects.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 1441–1452. [https://dl.acm.org/doi/10.1145/3540250.3558967](https://dl.acm.org/doi/10.1145/3540250.3558967)

[^4]: Chunqiu Steven Xia and Lingming Zhang. 2022. *Less training, more repairing please: revisiting automated program repair via zero-shot learning.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 959–971. [https://dl.acm.org/doi/10.1145/3540250.3549101](https://dl.acm.org/doi/10.1145/3540250.3549101)

[^5]: Spandan Garg, Roshanak Zilouchian Moghaddam, Colin B. Clement, Neel Sundaresan, and Chen Wu. 2022. *DeepDev-PERF: a deep learning-based approach for improving software performance.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 948–958. [https://dl.acm.org/doi/10.1145/3540250.3549096](https://dl.acm.org/doi/10.1145/3540250.3549096)

네 편 중 두 편을 아래 소개한다.

#### VulRepair: A T5-Based Automated Software Vulnerability Repair[^2]
CodeT5 에 실제 CVE 수정 이력 데이터를 학습 시키는 방법으로 취약점 자동 수정 도구를 구현했다.
Culint[^culint]와 유사한 학습 방식이서 이해하기 어렵지 않았다. 신기했던 것은 Culint 에 비해 훨씬
적은, 1% 수준의 데이터를 학습했는데도 효과가 있었다는 점이다. 정확도(Accuracy) 44% 를 달성했다고
한다. 미세 조정 학습에서는 오히려 적은 실제 데이터를 학습하는 편이 오버피팅을 피하고 이득을 취할 수
있을것 같다는 생각도 든다.

[^culint]: Yeonhee Ryou, Sangwoo Joh, Joonmo Yang, Sujin Kim, Youil Kim, *Code Understanding Linter to Detect Variable Misuse.* (Presented in ASE 2022)

#### Less Training, More Repairing Please: Revisiting Automated Program Repair via Zero-Shot Learning[^4]
CodeBERT 를 사용한 논문이었는데, 기계 번역 기반 자동 수정이 아닌 새로운 접근 방식이어서 새로웠다.
아이디어는 간단한데 Fault localization 을 이용해서 결함 위치를 찾아 Mask 처리한 뒤, 언어 모델의
Masked Token Prediction 기능을 이용해 결함이 없는 코드로 새로 채우는 것이다. 미세 조정 없이
CodeBERT 자체로 자동 수정에 사용할 수 있다는 장점이 있지만, Fault localization 기술의 정확도에
의존적이고 Expression 수준의 작은 수정만 지원되는 것으로 보인다.

대기업이 만들어둔 모델을 가져다가 약간의 미세 조정(Fine-tuning)으로 코드 수정이나 생성 기술을
구현하면, 성과가 대기업의 숨겨진 기술 덕분인지 연구진이 제시한 기술 덕분인지 알기 어렵다고 비판할
수 있다. 내가 학회장에서 만나서 이야기했던 사람들 중 기계 학습을 싫어한다고 말한 사람들은 이 문제를
지적했다. 특히 CodeT5 같은 경우에는 사전학습 코드를 공개하지 않고 있어서[^7] 공개된 모델을
미세조정하거나 그대로 사용하는 것 외에는 활용하는 데 제약이 있다. Codex 와 같이 학습 데이터가
공개되지 않은 경우에는 문제가 더 크다. 기술 간 비교평가에 사용하는 벤치마크 데이터가 이미 사전
학습에 사용되었는지 알기 어렵기 때문이다. 사전 학습에 사용되었을 경우 이미 알고 있는 데이터를
재생산한 것이므로 공정한 평가라고 보기 어렵다.

[^7]: "Can you release pre-training code of CodeT5?": [GitHub salesforce/CodeT5 Issue#40](https://github.com/salesforce/CodeT5/issues/40)

그럼에도 불구하고 프로그래밍 언어 모델과 트랜스포머를 활용하는 연구가 활발하게 진행되고 있다.
위에 언급한 논문 외에도 프롬프트 엔지니어링에 관한 논문[^8], 트랜스포머를 이용한 Call Graph Pruning
연구[^9] 등 다양한 방면으로 활용되고 있었다. 이 기술을 싫어하는 사람도 많고 논쟁의 대상이지만,
그렇기 때문에 연구가 더 발전할 수 있을 것이라고 기대한다.

[^8]: Chaozheng Wang, Yuanhang Yang, Cuiyun Gao, Yun Peng, Hongyu Zhang, and Michael R. Lyu. 2022. *No more fine-tuning? an experimental evaluation of prompt tuning in code intelligence.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 382–394. [https://doi.org/10.1145/3540250.3549113](https://doi.org/10.1145/3540250.3549113)

[^9]: Thanh Le-Cong, Hong Jin Kang, Truong Giang Nguyen, Stefanus Agus Haryono, David Lo, Xuan-Bach D. Le, and Quyet Thang Huynh. 2022. *AutoPruner: transformer-based call graph pruning.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 520–532. [https://doi.org/11.1145/3540250.3549175](https://doi.org/10.1145/3540250.3549175)


## 코드 리뷰와 프로그래머

이번에 직접 발표를 하지는 않았지만 회사에 있을 때 참여한 논문이 발표되었다. 사내 코드 리뷰 자동화
시스템을 소개하고 그에 대한 사내 사용자들의 반응을 조사한 논문이었다.[^10] 발표를 위해 삼성 리서치
권용휘님이 학회에 참석했다. 발표가 끝나고 예상보다 호의적이고 관심 있어하는 질문이 나왔다.
사람들이 코드 리뷰를 중요하게 생각하고있다는 느낌을 받았다.

[^10]: Hyungjin Kim, Yonghwi Kwon, Sangwoo Joh, Hyukin Kwon, Yeonhee Ryou, and Taeksu Kim. 2022. *Understanding automated code review process and developer experience in industry.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 1398–1407. [https://doi.org/10.1145/3540250.3558950](https://doi.org/10.1145/3540250.3558950)

Distinguished Paper 시상식에서도 이와 비슷한 인상을 받았다. 7편의 수상작 중 2편의 제목에 코드
리뷰가 포함되어 있었다. 한 편[^11]은 Meta 의 연구진이 낸 논문인데, 프로그래머가 코드 리뷰 요청에
대해 응답하지 않을 때 재촉하는 방법(Nudge)과 그 효과를 말했다. 다른 한 편[^12]은 코드 리뷰에서
보여주는 파일의 순서에 따라 코드 리뷰 코멘트 품질이 달라진다는 연구였다. 다소 직관적인 해석이라고
생각하지만 이걸 데이터로 잘 보여줬다는 데 의미가 있는 것 같다.

[^11]: Qianhua Shan, David Sukhdeo, Qianying Huang, Seth Rogers, Lawrence Chen, Elise Paradis, Peter C. Rigby, and Nachiappan Nagappan. 2022. *Using nudges to accelerate code reviews at scale.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 472–482. [https://doi.org/10.1145/3540250.3549104](https://doi.org/10.1145/3540250.3549104)

[^12]: Enrico Fregnan, Larissa Braz, Marco D'Ambros, Gül Çalıklı, and Alberto Bacchelli. 2022. *First come first served: the impact of file position on code review.* In Proceedings of the 30th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022). 483–494. [https://doi.org/10.1145/3540250.3549177](https://doi.org/10.1145/3540250.3549177)

코드 리뷰 관련 연구는 프로그래머 사이의 상호작용에 관심이 있다. 이런 연구가 중요하게 다뤄지는 데서
소프트웨어 엔지니어링이 사람에 관한 연구라는 것을 다시 느낀다.


## 교류 행사

이번 학회는 혼자 참석했고 발표 부담도 없었기 때문에 이 기회에 다양한 사람을 만나 이야기해보고
싶었다. 개회식에 공개된 통계 중 또 한가지 눈여겨본 숫자는 대학원생 수였다. 오프라인 참석자 약 400명
가운데 대학원생이 120명 정도 되었다. 앞으로 나와 같은 분야를 연구하고 경쟁할 사람들이 이만큼
되겠구나, 하고 가늠해보기도 했다.

오프라인 학회장은 모두를 외향형 인간으로 만드는 놀라운 공간이다. 처음 보는 사람과 이야기를 하고
있으면 또 다른 초면인 사람이 다가와서 내가 끼어도 되겠니? 하고 묻는다. 그런데 그렇게 끼어드는
사람들이 막상 얘기하다 보면 내성적인 사람인 경우도 많았다. 처음에는 혼자서 쭈뼛거리던 나도 시간이
지나갈수록 리포터에 빙의해서 처음 보는 사람들에게 많은 것들을 물어보고 다녔다.

계속해서 많은 사람들을 만나고 인사를 하면서 나와 내 관심사를 여러번 소개하게 되었다. 기본적으로
세가지를 소개하는데, 이름과 소속을 소개하고 관심있는 연구주제를 소개해야한다. 마지막 주제가
핵심이다. 이후 대화를 이어가는 주제가 되기 때문이다.

Newcomer’s Lunch 행사에서 다들 그걸 느꼈던 것 같다. 이 행사는 첫날 점심시간에 진행되었는데, 짧은
시간 동안 많은 사람을 만나게 하는 행사였다. 점심시간 내내 15분에 한 번씩 일어나서 자리를 바꾸고
처음 보는 사람과 이야기하면서 밥을 먹었다. 15분은 적당히 길고도 짧은 시간이었다. 이때 너무 큰
주제를 소개하면 서로가 무엇을 하는지 알아내기 위해서 더 자세한 질문을 하느라 시간을 보낸다. 너무
자세하게 소개하면 상세한 개념을 하나하나 설명하는데 시간을 다 써야 한다. 양쪽 다 이 조절에
실패하거나 서로 관심사가 너무 달라서 연구에대한 대화를 포기하면 남은 시간 동안 부산행을 봤다거나
가족이 BTS를 좋아한다는 이야기를 들을 수 있었다. 적절한 수준에서 서로의 연구를 이해하고 질문하는
연습을 할 수 있었다.


## 마치며

예전에도 한번 학회에 혼자 참석했는데 유신 교수님, 홍신 교수님, 김윤호 교수님 세 분이 챙겨주셔서 잘
지내다 온 기억이 난다. 이번에는 더 많은 한국인 교수님들이 계셨다. 첫날 저녁에는 유신 교수님께서
꼬치 구이와 맥주 모임에 초대해서 학회에 참석한 한국인 교수님들과 학생들을 소개해주셨다. 뱅킷에서
홍신 교수님, 탁병철 교수님, 김미정 교수님과 함께 식사했고, 오학주 교수님과 사파리 투어를 함께했다.
학회 기간 동안 챙겨주신 교수님들께, 그리고 반겨준 다른 학생들에게도 감사드리고 싶다. 회사에서
코드리뷰봇 연구 개발을 함께했던 발표자 권용휘님과, 김택수 박사님을 포함한 다른 저자분들께
감사드린다. 무엇보다도 이 모든것을 즐기고 배울 수 있게 지원해주신 허기홍 교수님과 연구실에
감사드린다.


#### 참조
