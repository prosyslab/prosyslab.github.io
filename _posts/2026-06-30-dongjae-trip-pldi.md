---
title: AI 시대에 PL을 연구하는 대학원생의 고민
date:   2026-07-12
author: Dongjae Lee
kor_author: 이동재
tags:
  - Trip
  - PLDI2026
classes: wide
---

## 들어가며

운 좋게도 PLDI에 논문 한 편을 출판하게 되어, 올해 학회에 참석할 기회를 얻었다.
이번 PLDI는 미국 콜로라도주의 작은 대학 도시 볼더에서 열렸다.
볼더는 날씨가 좋아 옷차림과 짐도 평소 여행보다 가벼웠다.

학회에서 중요한 것은 발표 자체보다 쉬는 시간과 식사 시간에 나누는 이야기인 것 같다.
발표가 이미 지나간 일에 관한 것이라면, 식사 시간의 대화는 앞으로 해야 할 일에 관한 것이기 때문이다.
그런 점에서 이번 PLDI의 핵심 주제는 AI였다.
세 편의 기조연설 가운데 두 편이 AI를 다뤘고, 평소 대화도 대부분 AI가 공통 주제였다.

AI가 일으킨 거대한 변화 속에서 프로그래밍 언어 분야는 어떻게 고유한 가치를 지키고, 어떤 역할을 맡아야 할까?
이 글에서는 볼더에서 직접 보고 들은 경험을 바탕으로, PL을 분야의 대학원생으로서 그 질문에 대한 답을 일부나마 남기고자 한다.

<table style="width:100%; table-layout:fixed;">
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNUGDKn_P-47WnxxI4IXsLRH41cqG3zh9D2SDfQtQG4C2qFE86A7QjKiDkSLW0GDo2KrnP_HIFiDmGIXsTTiLp49R9e9w1G3agyYVq0MnpwqlpWQU8KjRRcCX37jfTINKLD-mMq5snzFRLsoEcRhQJ6=w1239-h929-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>맛있는 대한항공 기내식</b></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczOZDC7OFWLQ35WdLImM5fGTKp5n6tDYTHI6xU04jXNrnhEbnt1Zv36MieVVNo-zC4vA1hlkIhgup-CaT0VSNbsR0pP77UEczbFpNYFEN6D15EhIGwWEvKy8ecWpUSZAB7NGrWG1v47CNrYHIGnjxyfk=w697-h929-s-no-gm" /></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>멋진 로키 산맥</b></td>
    </tr>
  </tbody>
</table>

## 볼더로 가는 길

콜로라도주 볼더는 미국 내륙에 자리한 소도시로, 한국인에게는 비교적 낯선 곳이다.
덴버에서 차로 한 시간 거리에 있지만 덴버행 직항편이 없어, 시애틀을 경유해 약 20시간 만에 도착했다.

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczMwv1UlmIpB8rccQeSLX5vjdq1Rt_8PQoRFki_i2d66CfpOjNZKtJ9i6Bqr_WLQBTJnv8rNo1LvomSoPWtHyBIhWtH5SuvorywTZEX8Dz0vzegeKM4Ux28Sk65RXP2v0CHsJxP3jWMeQJFYzgUHQqUg=w697-h929-s-no-gm?authuser=0" /></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>멋진 호텔 풍경</b></td>
    </tr>
  </tbody>
</table>

학회장은 신축 호텔인 Limelight Boulder였다.
호텔 너머로 펼쳐진 로키 산맥이 인상적이었다.

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNJKrtbuaOzGwFbJi2hbE14FgYqLFx4Joas_RmdVSw3OaF2r1EngzZrTOio5ccYCsO5j-cvsu9s1S2bJ3gLHzVV1qhKu2fgT65DeM0tSLWIom63YnNOUi6AJ-dSaNvA6fM7A6oD8IoPo5JCe1iCHzdu=w1239-h929-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczPxEINo-sU2T9mL95PNaV1khpnFxe5QRw5cX8kRvyDlQRKT0XKjPJCCgk1CU7Rg6AyeAMN_8rjZTII16V6esJBrgGZiZTS3CBAT3_Ofbq6uEpau753Y_g044J_WVtRLa5EB-nvDO_cGJwkv3zaCqBki=w1239-h929-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczMM3rUMg-J1WMXG-WVD4-1FXRv49Rq1HBv_duq7TSNggNrQyx_hd7Zvl8ZdeeJse1NG0uZlvQ2i4l7JO4Ufuc5ZXDsfBea0UAPssQ1k1OzdYacYOUKAeCNhMlDVnnw8bToP-g3E4TdELI7jnZU7Fvor=w1239-h929-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="3"><b>맛있는 호텔 조식. 차례로 프렌치 오믈렛, 볼더 브렉퍼스트, 에그 베네딕트다.</b></td>
    </tr>
  </tbody>
</table>

조식이 별도로 제공되지는 않았지만, 1층 레스토랑에서는 팁을 제외하고 약 20달러에 한 끼를 먹을 수 있었다.
달걀 요리와 감자가 어우러진 전형적인 서양식 아침 식사였다.

## PAgE

첫날에는 PAgE 워크숍에 참석했다.
PAgE는 에이전트를 위한 여러 PL 접근법과 PL을 위한 에이전트 기반 접근법을 함께 다루는 워크숍이었다.
PLDI에서도 에이전트 관련 워크숍이 열릴 만큼, 이제 AI의 영향이 미치지 않는 곳을 찾기 어려워 보였다.

내용 자체는 이미 논문으로 접한 것이 많아, 새롭게 다가온 부분은 많지 않았다.
그러나 PLDI에서 이러한 워크숍이 열렸다는 사실만으로도 변화의 신호는 분명했다.
작년까지만 해도 PLDI에서 AI를 활용한 방법론을 찾기 어려웠지만, 올해는 AI를 주제로 한 별도 워크숍까지 마련되었다.
PLDI가 AI를 한층 적극적으로 받아들이고 있다는 인상을 받았다.

Gagandeep Singh 교수님의 기조연설도 인상적이었지만, 가장 기억에 남은 대목은 Microsoft 연구팀이 소개한 Verus Agent 구축 과정의 실패담이었다<sup>[1](#autoverus)</sup>.
Microsoft는 2023년부터 Rust 프로그램을 검증할 수 있도록 확장한 언어인 Verus를 위한 에이전트와 평가 벤치마크를 구축해 왔다.
그 결과 AutoVerus라는 에이전트 고삐(agent harness)를 개발해 좋은 성과를 거두었다. 여기서 ‘고삐’는 에이전트의 동작을 제어하고 보조하는 소프트웨어를 뜻한다.
그러나 언어 모델이 빠르게 발전하면서 Opus-4.8과 범용 고삐인 Copilot을 결합한 매우 단순한 접근법이 AutoVerus의 성능을 압도했다.
모델의 역량이 커지자 에이전트를 제어하던 고삐가 오히려 성능을 제한하는 장치로 작용했기 때문이다.
결국 모델의 역량이 커질수록, 그에 맞춰 고삐의 크기도 알맞게 조절해야 한다.

문제는 OpenAI와 Anthropic 같은 영리 기업이 언어 모델의 발전 방향을 주도한다는 점이다.
이들은 자사의 에이전트 고삐인 Codex와 Claude Code에 맞춰 언어 모델을 훈련하고 출시한다.
반면 외부 연구자는 모델의 학습 방향을 직접 통제할 수 없다. 새 모델을 직접 사용하며 무엇을 잘하고 어디에서 실패하는지 계속 확인할 수밖에 없다.
처음부터 불리한 조건에서 벌이는 경쟁인 셈이다. 모델 버전이 바뀌면 기존 고삐를 전면 폐기해야 할 수도 있다.

이런 이유로 Microsoft도 고삐 설계를 잠시 미뤄 두고 소형 모델의 미세 조정(fine-tuning)에 집중하는 것으로 보인다.
소형 모델을 훈련하는 이유는 비용 문제 때문이다.
현재 프로그램 검증에는 테스팅보다 훨씬 많은 비용이 든다.
값비싼 GPT나 Claude 대신 쉽지만 반복적인 검증 작업을 수행할 소형 모델이 필요한 것이다.
그러나 소형 모델의 미세 조정조차 대학 연구실이 감당하기에는 비용이 크다.
특히 최근에는 미세 조정보다 훨씬 값비싼 실시간 강화 학습(online reinforcement learning)이 주목받으면서 자원이 부족한 연구자에게는 연구의 진입 장벽이 빠르게 높아지고 있다.

그렇다면 충분한 자금도, A100·H100·B100 같은 고성능 GPU도 없는 PL 연구자는 무엇을 해야 할까?
한 가지 길은 근본 원리에 집중해 에이전트 고삐를 설계하는 것이다.
새 모델이 나올 때마다 기존 고삐를 폐기해야 하는 까닭은 고삐의 기능 대부분이 휴리스틱에 의존하기 때문이다.
휴리스틱은 설계할 때 전제한 조건이 유지되는 동안에는 잘 작동한다. 그러나 모델이 바뀌어 그 전제가 무너지면 쓸모를 잃고, 오히려 성능을 떨어뜨린다.
따라서 휴리스틱에만 기대기보다 수학적 정당성을 보일 수 있는, 다시 말해 튼튼함이 검증된 고삐를 설계해야 한다.
Lean과 같은 증명 보조기(interactive theorem prover)에 기반한 검증 기법들이 AI 분야에서 주목받는 이유도 휴리스틱을 넘어서는 수학적 근거를 제공하기 때문이다.

## (쉬어가기) 로키 산맥 하이킹

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczO3x0RKPaLPSeVVsh5XSoHaHWXXBIK0BrB92FSa1VqlI3fhGASjhPWukgh6jkAWLBYBKaQzK8Ck8uak9ySZ8hqLT-ULugTTye6BBFC9ouN0WVwxxeONmdevfK8hEzSvvScR75XX97g1-dTWlrDNfEjYvw=w1238-h929-s-no-gm" /></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>볼더를 배경으로 로키 산맥에서</b></td>
    </tr>
  </tbody>
</table>
<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczPO0Ow1BaRqr66qa6J0L5IAJohXoyuk6jliHEJa2GfTlcVFQRuIYSiLzV6_qqmit2O6fxaBi60Ovz7LnuqgM78tPzqKhFjeDBNMyNqkQfprOO8S5fxAGWg4Z1bllxoiNwODqG1Utwpok4OURKcpQ2At=w697-h929-s-no-gm" /></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>로키 산맥을 배경으로 볼더에서</b></td>
    </tr>
  </tbody>
</table>

이번 PLDI가 콜로라도주 볼더에서 열린 만큼, 로키 산맥 하이킹은 자연스럽게 일정에 포함되었다.
주최 측이 교류 행사로 단체 하이킹을 마련해 준 덕분에 좋은 코스를 걸을 수 있었다.
왕복 한 시간 남짓한 길을 걸으며 이탈리아에서 온 석사과정 학생과 친해질 수 있었다.
북적거리는 서울과 달리 자연을 가까이에서 즐길 수 있는 환경이어서, 느긋하게 이야기하며 네트워킹하기 좋았다.

## PLMW

작년에 이어 올해도 PLMW(PL 멘토링 워크숍)에 참석했다.
작년과 달리 학생들의 친목을 위한 행사, 이를테면 금지어 게임 같은 프로그램은 사라졌다.
아마 참가자들의 피드백이 반영된 결과인 것 같다.

PLMW는 처음부터 끝까지 강의 형식으로 진행됐고, ‘연구하는 방법’에 관한 이야기가 주를 이루었다.
가장 눈길을 끈 세션의 제목은 "Roses are Blue, Violets are Red; With Future AI, is Research Dead?"였다.
AI가 모든 인지 작업을 자동화할 수 있다는 담론이 힘을 얻는 오늘날, 연구 자체의 의미는 연구자라면 누구나 한 번쯤 묻게 되는 문제다.
아쉽게도 세션은 이 문제를 직접 파고들기보다 연구 주제를 선별하고 구성하는 여러 방법론을 소개하는 데 초점을 두었다.
그럼에도 연구자라면 지적 노동의 자동화가 현실이 된 세계에서 연구의 본질을 다시 살펴볼 필요가 있다.

개인적인 생각을 덧붙이자면, 방향을 제시하는 일은 여전히 인간의 영역으로 남겠지만, 구현과 반복 작업의 상당 부분은 AI가 맡게 되리라 본다.
목표가 명확하고 결과를 검증할 수 있는 작업에서 AI 에이전트는 이미 많은 인간보다 뛰어난 성능을 보인다.
최적화나 기능 구현 같은 작업에서 인간은 AI의 지치지 않는 반복 수행 능력과 방대한 맥락 처리 능력을 따라가기 어렵다.
반면 거시적인 방향을 제시하고 중요한 문제를 찾아 정의하는 일은 아직 인간의 몫에 가깝다.
인간이 모호한 문제를 정교하게 다듬어 검증 가능한 형태로 바꾸고, AI가 반복적인 실행과 정리를 맡는 분업이 가능하다.
여기서 방향을 제시한다는 말은 단순히 AI에게 할 일을 분배하는 일이 아니다.
수많은 가능성 가운데 지금 풀 가치가 있는 문제를 고르고, 왜 그것이 중요한지 판단하는 일에 가깝다.

다만 그 과정에서 아이디어를 검증하는 속도는 훨씬 빨라지고 경쟁은 더욱 치열해질 것이다.
AI가 기존 접근으로는 충분히 설명하거나 해결하기 어려운 결과를 더 일찍 드러낸다면, 패러다임의 전환과 큰 발전이 일어나는 주기도 빨라질 것이다.
이는 학계와 인류 전체의 발전이라는 관점에서는 바람직한 흐름일 수 있다.
그러나 그 한가운데서 일하는 개인은 급격한 변화와 치열한 경쟁으로 더 큰 피로를 느낄 수 있다.
오늘날 많은 연구자가 느끼는 불안도 지나치게 빠른 변화 속에서 뒤처질지 모른다는 두려움, 곧 FOMO에서 비롯된다고 생각한다.

## (쉬어가기) 건강한 몸에 건강한 정신이 깃든다

건강한 신체를 유지하는 일은 연구자로 오래 일하기 위한 필수 조건이다.
인턴 시절과 대학원 초반에 겪은 스트레스로 몸무게가 이전보다 20kg 이상 늘어난 적도 있었다.
당시에는 실력이 부족한 상황에서 평소처럼 운동하는 것을 사치라고 생각했다.
지금 돌아보면 학부생으로서 경험과 실력이 부족한 것은 당연한 일이었는데도, 조급한 마음에 운동을 거의 하지 않았다.
그러나 체력이 떨어지고 스트레스에 대한 저항력도 약해지자, 오히려 원하는 만큼 집중하기 어려워졌다.
다행히 지금은 체중 관리와 운동을 통해 건강한 체중을 유지하고 있다.
과거로 돌아갈 수 있다면, 아무리 바쁘더라도 운동만큼은 꾸준히 이어 갈 것이다.

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczMuuTZpD7te_Fn4C6LDXvCBindM4ZDwgb7vx8dYe5aQPDCLKiZCFOUi9grL3vANQsioic5zf_ujq19tZWatAap1x4aJGU-iDItbq1rRhUwthKvftAaz94Nlr8fn6FNW5x9Mr7MQBq7rU60fwLmCpGji=w1078-h1436-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNxs7m3yfB_JDMdnsagCTHKZ0rQdDQBmefeNuEegFhhIxiyZzzzTnNYSGT3KWBd3H7tFFJ0OIQFUUzUvjxE91FP20mNLeupKIRNCUmKRfWlnuCcftWU3Eqdy4Z7hMLyvHQQB2ppZwuSPhJrYZRrtdN9=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>월요일과 화요일 오전에 방문한 호텔 내부 헬스장. 크기는 작지만 알차게 구성되어 있었다.</b></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczO6Y8lDTg33NbGHZRn2KjSMVdodIt5olaS0XWsXsLKBKQSVlDINq29Ki1z3SAbZVRwKV6CZQi5DxYwbf3JUZ0nKFvl5SMrfNOATN4-LlxZJJ42bpMSk9WJb5RRPBkMbzLI0iO9nxEn2L5_kDnGb0k_f=w1078-h1436-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczO1Y0WdDRzwm0R-X1jVhRNzD0d-TY5mqLdtyyLFKYK5bBSm43U1eT6fv7xortaP7V0u08FzrVxaHF4lCEWD-uwScYH4LASidyWOF10Akbs6LtxHf4Ent17L6jbYnFB_DIO9onWrqdT3rdxvreyZZR7d=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>둘째 날 학회 일정을 마치고 방문한 호텔 수영장. 멋진 노을과 로키 산맥이 어우러진 풍경이 인상적이었다.</b></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczN9ls_ifUGeIyS1Wk0x0oXpnZ_PAUUpcKWWEJ5BPBPt6x0XChHeip_1vqSbO9cXHkJ_8639lbuB43xb3yVvESR7vkm2edpn2Ff6hRpAfF6TTr2FPbpMEC6l7axARZdK9nkszuIb5X9jl5rVeLuxf81q=w1914-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>셋째 날 류석영 교수님 연구실 분들과 함께한 러닝. 고산지대여서 그런지 평소보다 훨씬 힘들게 느껴졌다.</b></td>
    </tr>
  </tbody>
</table>

## Expecto

<table>
  <thead>
    <tr>
      <th style="text-align: center;" colspan="2"><img src="https://lh3.googleusercontent.com/pw/AP1GczOfkVZPkpVXer4xOpoiOPmuOS7VULPSG-rwUTDm9Xl_MMQubMFZ7cn_swzdT77kUTVGipq08GfcEU88P4ikt2cx-VIeMeUfppPkU2VPhOV9Op2XOGEDKnxzPxTAQoMxqgOvA1PcT_1dRK_pK16Wsy-sSA=w1914-h1436-s-no-gm"/></th>
    </tr>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczMMceB0OEeUHni5ahOJagVhdnX7VJsdA9ncYimTptI2IyLYCI3p7EMD-3v-nC-2Af6fk_Wpp9tkInYLmSVeEb7NIKVwsKpctXy0DK8BuRfR5H8sC7N-7vaz1eqvLdAa6qkKTQyUBl4tmSHraFhTyGX7vg=w1078-h1436-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNsT0exZnUSPDgTiYZ9n0OknUEzUaLw8Prlc9vmTwJuXSA7kZwBND85MK5b_TkUKOo_sLG7SXyKHRvtWQRM6ziTjpV39KNv89k7IQG_KfMZzx93nZbaJtzP72nKeSgk82WyBoS8DVgNQKqz2F06bswX9Q=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>교수님께서 찍어 주신 Expecto 발표 사진</b></td>
    </tr>
  </tbody>
</table>

수요일은 본 학회 첫날이자 내가 처음으로 PLDI에서 발표하는 날이었다.
작년 MobiCom에서 첫 국제 학회 발표를 경험했지만, 여전히 긴장되기는 마찬가지였다.
특히 이 연구에는 MobiCom에서 발표한 VeriSafe Agent보다 더 깊은 애착이 있었기에, 잘하고 싶은 마음도 컸다.

발표를 열심히 준비했지만 아쉬움은 남았다.
긴장한 탓에 더 구체적으로 설명해야 할 부분을 지나쳤고, 질의응답 시간에는 질문에 온전히 집중하지 못해 충분히 답하지 못했다.
이런 자리일수록 힘을 빼고 긴장을 내려놓아야 준비한 만큼 실력을 발휘할 수 있다.
그러나 내게 중요한 자리인 데다 아직 익숙하지도 않아 마음처럼 쉽지 않았다.

다행히 청중의 반응을 보니 내가 전하려던 바는 대부분 전달된 듯해 마음을 놓았다.
특히 월요일과 화요일에 만나 발표에 초대했던 사람들이 실제로 찾아와 축하해 주었고, 발표가 흥미로웠다는 말도 건넸다.
그 순간 묘한 소속감을 느꼈고, 네트워킹과 학회 발표라는 두 목표를 모두 이룬 듯해 기뻤다.
내게 이번 발표는 연구 결과를 소개하는 일 이상이었다.
오랫동안 애착을 둔 연구를 PLDI에서 발표하고, 그 연구를 매개로 사람들과 대화를 나누면서 내가 이 공동체의 구성원이 되어 가고 있음을 실감한 순간이었다.
작년 서울에서 열린 PLDI에서는 논문을 발표할 기회도 없었고, 네트워킹도 어색해 제대로 하지 못했다.
그때와 비교하면 1년 사이에 나름의 성장을 이룬 듯해 만족스러웠다.

발표 뒤에는 내 논문에 가장 큰 영향을 준 Microsoft의 Shuvendu Lahiri와 점심을 함께했다.
Shuvendu의 연구팀은 현재 명세와 인간의 의도를 일치시키는 방법에 큰 관심을 두고 있다고 했다.
그 관심의 바탕에는 AI와 엄밀 검증(formal verification)의 진정한 병목이 명세 작성에 있다는 문제의식이 자리하고 있었다.
Expecto 역시 같은 관찰에서 출발한다. 자연어로 표현된 의도에서 명세를 생성하는 문제를 하향식 명세 합성이라는 아이디어로 풀어낸 연구다<sup>[5](#expecto)</sup>.

다만 명세에는 기능적 요구 사항뿐 아니라 성능, 코드 품질, 보안과 같은 비기능적 요구 사항도 담겨야 한다.
아직 이러한 속성을 효과적으로 표현하는 방법이 충분히 마련되지 않았기에, 명세 언어의 확장은 앞으로 프로그래밍 언어 분야의 주요 연구 주제 가운데 하나가 되리라 생각한다.
Expecto처럼 자연어로 표현된 의도에서 명세를 생성하려는 연구도 앞으로 늘어날 것이다.
그러나 완벽한 해법을 마련하기 어려운 문제인 만큼, 앞으로도 중요한 과제로 남을 것이며 공학적인 관점에서 접근하는 일이 중요해 보인다.

앞서 설명했듯이 인간은 모호한 문제를 명료하고 검증 가능한 형태로 바꾸어 에이전트에게 위임하는 역할을 맡게 될 것이다.
다시 말해, 인간의 핵심 역할은 명세를 작성하는 일이다.
명세 작성은 AI 에이전트를 제대로 다루기 위한 핵심 기술이 될 것이다.
나아가 프로그래밍을 넘어 여러 분야에서 에이전트가 인간의 의도를 정확히 수행하도록 이끄는 기술로 자리 잡으리라 본다.
프로그래밍 언어 기술이 앞으로 소프트웨어 개발자뿐 아니라 에이전트를 다루는 모든 사람을 위한 기술로 확장되어 더 많은 관심을 받기를 바란다.

## Expecto 비하인드 스토리

Expecto는 주제 선정부터 마무리까지 교수님과 내가 함께 진행한 연구다.
어쩌면 내가 박사과정에 진학하게 된 출발점이라고도 할 수 있다.
2년 전 겨울, 석사 1년 차가 끝나 갈 무렵 나는 박사과정 진학 여부를 두고 깊이 고민하고 있었다.
당시 진행하던 연구에 많은 노력을 기울였지만 큰 진척은 없었고, 더 오래 붙들어도 상황을 바꿀 만한 돌파구는 보이지 않았다.
그래서 연구를 적절히 마무리한 뒤 졸업할지, 아니면 다른 주제로 전환해 박사과정을 밟을지 고민했다.

진행하던 연구를 잠시 접어 두고 새로운 주제를 찾아 나섰다. 마침 추론 모델(OpenAI의 o1 모델)이 등장하며 LLM이 또 한 번 도약하던 시기였다.
당시 LLM을 둘러싼 주된 비판은 GPT-4o와 같은 모델이 추론하는 것이 아니라 패턴을 맞추는 데 그친다는 것이었고, 나 역시 그런 측면이 있다고 생각했다.
그러나 추론 모델은 이러한 비판에 정면으로 답할 만큼 놀라운 성능 향상을 보여 주었다.
나는 LLM의 발전이 당분간 멈추지 않으리라 생각했고, 이를 활용한 연구를 하고 싶었다.

그때 눈에 들어온 것이 엄밀 검증(formal verification)이었다.
엄밀 검증은 프로그램이 주어진 성질을 만족한다는 사실을 수학적으로 보장한다는 큰 장점이 있다.
그러나 많은 노동력이 필요해 극도로 중요한 소프트웨어가 아니면 좀처럼 시도하기 어려운 방법이었다.
LLM의 비약적인 발전으로 엄밀 검증의 자동화가 가능해 보이자 많은 사람이 이 분야에 뛰어들기 시작했다.

문제는 엄밀 검증에 엄밀 명세(formal specification)가 필요하다는 점이다.
그러나 당시에는 엄밀 명세가 이미 주어졌다고 가정하거나, 주어진 코드에서 엄밀 명세를 합성하는 연구가 주로 진행되고 있었다.
나는 자연어에서 엄밀 명세를 정확히 생성하는 기술이 필요하며, 이 과정이 핵심 병목이 될 것이라고 예상했다.
운 좋게도 다른 연구자들도 엄밀 명세에 관심을 기울이기 시작했고, 시기가 맞아떨어져 2026년 PLDI에 논문을 발표할 수 있었다.

## (쉬어가기) 귀여운 콜로라도 토끼

콜로라도 대학교 캠퍼스에서 만난 귀여운 토끼다.
미국 토끼는 크고 무섭게 생겼으리라 막연히 생각했지만, 의외로 친숙하고 귀여운 모습이었다.

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNLN3RJ1GDC4WNMFhN5CUqz7xAvVfD3123U-yd3YBvf_DkOa5ylZOJMnnGD-36UmXehRmjy-CsFJ2ZVKcKtp1KPHmqPerRPimNtmSbSifabNflwfJ0_WSJ-MbJN2TPTBQtXG2jYtsJVPbHAfzxUgB8e=w1204-h1604-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>귀여운 토끼</b></td>
    </tr>
  </tbody>
</table>

## 새로운 병목은 검증

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczPgzzuEPFxx-2kdc8gjQ2Lyqyx30j04eCf1yx4WgoTkJ-u0eyD5JBl2v1EjEFHQ-7HLmYa6x4UYtxhRn6tk0kvd3SV0w8HOoi3SHNOz0Vzs5x0c9EmxoUNw9u9XQreyu56VZC3IcIn4_-SqCsiUUsGQ=w1204-h1604-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczOq6GOpdSFWLgSdkkFJkBvWSog2yIqvRmApgl3MAjtc3Tyacd9iNGdxLWOlbfixeEtFDFrCMt2f6PrS6QNaCWsQCPoCDDSQeRK7Jfhqf4o22ToPscaMI69DSpV672HEfERAsSC-Io0Fa-_a1yFNcj1U=w1204-h1604-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>이제 검증 연구가 핵심이다</b></td>
    </tr>
  </tbody>
</table>

목요일은 UCAL 김미령 교수님의 기조연설로 시작되었다<sup>[3](#miryung-kim)</sup>.
핵심 주제는 프로그램 작성이 아니라 검증이 새로운 병목이 되었으며, 이 과정에서 속성 기반 테스팅(property-based testing)이 어떤 역할을 할 수 있는가였다.

의도에 맞는 프로그램을 자동으로 합성하는 것은 컴퓨터 공학 분야의 오랜 숙원 중 하나였다.
PL 분야에서는 이를 위해 SyGuS, CEGIS 등 여러 합성 방법론을 개발해 왔다.
그러나 프로그램 합성에서는 PL 분야가 AI에 주도권을 내주었다.
그 과정에서 얻은 여러 아이디어는 여전히 유용하겠지만, 프로그램 합성 문제만 놓고 보면 SOTA 합성기조차 최신 AI 에이전트의 프로그램 생성 능력을 따라가지 못한다.

이견의 여지는 있겠지만, 특수한 상황을 제외하면 일반적인 프로그램 합성 문제는 LLM에 의해 대부분 해결되었다고 본다.
이제 핵심은 합성할 문제를 정의하고, 합성된 프로그램이 올바른지 확인하는 일로 옮겨 갔다.
즉, 명세 작성과 구현이 그 명세를 따르는지 증명하는 일이 중요해졌다.

앞서 명세 작성의 중요성을 길게 이야기했으므로, 여기서는 증명에 초점을 맞추고자 한다.
증명은 프로그램 합성과 비슷한 문제이지만, 합성보다 변화에 취약하고 비용도 많이 든다.
증명이 제공하는 것은 올바름에 대한 보장이지 새로운 기능이 아니다. 그러나 그 비용은 테스팅보다 압도적으로 크다.
테스팅과 달리 코드나 의도가 바뀌면 함께 수정해야 하는 부분도 훨씬 많다.
이 점이 프로그램 검증을 실제 산업에서 활용하기 어렵게 만든 핵심 이유 중 하나다.
하드웨어와 달리 소프트웨어는 쉽게 바꿀 수 있고 끊임없이 변화한다. 이는 소프트웨어의 핵심 특성이자 장점이다.
하지만 프로그램 검증의 관점에서 소프트웨어의 변경은 증명하려는 명제 자체가 달라진다는 뜻이다. 따라서 검증 결과는 변화에 매우 취약하다.

김미령 교수님의 핵심 아이디어는 비용이 큰 검증을 무작정 수행하는 대신, 속성 기반 테스팅으로 구현이 명세를 만족한다는 확신을 어느 정도 얻은 뒤 검증하자는 것이었다.
이 이야기를 들으며 앞으로의 과제는 검증을 이상적으로 완전하게 만드는 데만 있지 않다고 느꼈다.
개발 과정에서 감당할 수 있는 비용으로 신뢰를 높이는 실용적인 검증 방법을 찾는 일도 그만큼 중요하다.
구현체가 이미 있는 상황에서는 좋은 해결책이다.
그러나 구현체가 없거나 구현체와 증명을 함께 변경해야 하는 상황에서는 어떨까?

구현체와 증명이 모두 없는 상황에서는 둘을 동시에 생성하는 알고리즘이 가장 효과적일 것이라고 예상한다.
다만 기존 규칙 기반 합성(deductive synthesis)과 같은 합성 방식은 대규모 프로그램을 생성하는 데 한계가 있다.
대규모 프로그램을 생성하려면 LLM의 도움이 필요하며, 이때 LLM을 애초부터 올바르게 만드는(correct-by-construction) 합성 알고리즘에 잘 녹여 내는 것이 핵심이 될 것이다.

## Jane Street도 엄밀 검증을 한다!

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczOK5ojzq3tr2_ICmTceTTqGXAsFGTg2feEB6eAx26uXSDqJce4ngPE7Wq4UUNmHt5wErNgdxc5D3r3RZ-aeeQvEhI--7dWXMIhEb-JO9EYlwtXHiqjHMURipKfrwpDCdGrgKoa4t-IzcOQoSgPRBjAt=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>Jane Street가 개발한 OCaml 확장판 OxCaml</b></td>
    </tr>
  </tbody>
</table>

Jane Street는 소스 코드 대부분을 OCaml 기반으로 작성하는 거의 유일한 회사로 알려져 있다.
사실상 OCaml과 관련 생태계의 거의 유일한 후원자라고 할 수 있는 고마운 회사다.
학회 부스에서 Jane Street가 엄밀 검증에 관심을 두고 있다는 이야기를 듣고, 그 배경을 들여다보았다.

Jane Street는 초기 접근법으로 특화 모델을 직접 훈련하기보다 GPT, Claude에 자체 제작 언어와 에이전트를 결합하는 방식을 고려하고 있었다.
특화 모델을 개발하더라도 GPT나 Claude의 새 버전이 나오면 더 뛰어난 성능을 보일 가능성이 매우 높기 때문이라고 했다.
Codex와 Claude는 생소한 언어인 OxCaml도 매우 잘 다뤄, 자체 모델 훈련에는 큰 관심이 없는 듯했다.

Lean이나 Rocq이 아니라 Dafny와 같은 Hoare Logic 기반 검증 도구를 선택한 이유도 물었다.
수학 문제를 증명하는 것이 목적이 아닌 만큼, 코드 검증에는 이 방식이 더 적합하다고 판단한 듯했다.
앞으로 엄밀 검증 분야의 채용도 진행할 예정이라고 했다.

Jane Street처럼 투자 대비 효율을 중시하는 퀀트 회사가 PL과 엄밀 검증에 관심을 가진다는 사실은 놀라우면서도 반가운 일이다.
수동 엄밀 검증은 투자 대비 효용이 매우 낮은 기술이지만,
AI가 생성의 진입 장벽을 크게 낮추면서 자동화된 엄밀 검증이 실용적인 기술이 되어 가고 있다는 생각이 든다.
그 과정에서 PL 커뮤니티가 많은 기여를 할 수 있기를 기대한다.

## (쉬어가기) 볼더 시내 탐방기

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczOtDWbQ0Tl-3SEl-eu613Dq5uJzEcKCKbgT30yQ82eseB6yHRL4jA5ZKYO70V_W0dTuND8_fjyLefNcO6k9UNMVbWXD0JlV3xWc7BEQr6Q6adOKZFE-yiqAtIv4xZxrWZ1zLmTO4thSG7CYrKeGDfhQ=w1078-h1436-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczPMmuDU9bhzQGOBDpto1qFkFFJ_30d5TJKhis5iAzaPsoCrhDGFmh_PP5UsAZjroFIwBQ6P7OxWgeZHQm32DtVPqwkX4R3pybfxRg0PABXYkPw6NtvXlSZnWmMzbrj98vfEignjynu2vpHeXTJv1Uoz=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>볼더 시내의 낮과 해 질 무렵</b></td>
    </tr>
  </tbody>
</table>

학회 기간에 볼더 시내를 두 차례 찾았다.
시내는 호텔에서 걸어서 15~20분 정도 거리에 있었다.
한 번은 류석영 교수님 연구실 분들과 저녁에 펍을 찾았고, 다른 한 번은 기념품을 사러 갔다.

펍으로 가는 길에 한 볼더 주민이 꼭 노을을 봐 달라고 권해 사진을 한 장 남겼다.
그는 이 노을을 보기 위해 볼더에 산다고 말했다. 실제로 로키 산맥을 배경으로 펼쳐진 볼더의 노을은 장관이었다.
날씨가 대체로 쾌청해 구름이 없거나 얇게 낀 날이 많았고, 덕분에 노을을 감상하기에 더없이 좋은 하늘이 펼쳐졌다.

시내에는 붉은 벽돌로 지은 2층 건물이 일렬로 늘어서 있었다.
건물의 디자인이 하나같이 비슷해 테마파크의 한 구역 같은 느낌도 들었다.
눈에 띄게 특별한 곳은 없었지만, 관광객으로 보이는 사람들로 예상보다 붐볐다.
거리에는 관광객을 위한 기념품점과 옷가게, 음식점이 주로 자리하고 있었다.

기념품점에서는 자석과 콜로라도 대학교 티셔츠를 사려고 했다.
하지만 티셔츠가 정식 상품처럼 보이지 않아 사지 않았다.
나중에 콜로라도 대학교 학생에게 자신도 시내 기념품점에서 티셔츠를 산다는 말을 듣고, 그때 살 걸 그랬다는 아쉬움이 남았다.

## PLDI에 대한 비판과 나의 생각

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNkcy7LYN5pCATpcghneVlzzsYChvTBilMX_0l3pRwjGhTLE6lpEjkNn_gZ5RYm_m-HAZS5hfDBMsjBrSwXxkq9IOFJzPUWMBJv2lsdFkeeYrz5Oy245Yv95z3ny6ADsItCbD_mFdJmjt2tvC7hywPY=w1078-h1436-s-no-gm"/></th>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczNtkz8DSbdp5rBPOwf8u_yDrpdElg5McBbNKc-ENHCURpuditF1LGvUd_pT99XMZRWiYxqxubxQ-d1VQur162BbPcJgg7v5wSdaplix2NKWtP16E6BB-xzO8WiJFErcHVtsmrYmUUpyDIwidWWIkJVS=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center" colspan="2"><b>PLDI, 너무 까다롭게 굴지 마라</b></td>
    </tr>
  </tbody>
</table>

학회 첫날 MIT의 Saman Amarasinghe 교수님은 기조연설에서 PLDI가 새로운 연구에 지나치게 배타적이라는 비판을 제기했다<sup>[2](#saman-amarasinghe)</sup>.
요지는 최근 AI 컴파일러 분야의 중요한 논문들이 PLDI가 아닌 ASPLOS, SOSP 같은 OS·시스템 학회에 출판되고 있다는 것이었다.
게다가 이런 논문들은 PLDI에서 좋지 않은 평가를 받아 시스템 학회로 쫓겨나듯 옮겨 간 논문들이었다고 한다.

새로운 연구에 배타적인 태도는 학회 논문의 품질을 관리하는 데 양날의 검이 된다.
새로움에 신중한 태도는 저품질 논문을 걸러 내는 유용한 휴리스틱이 될 수 있다.
방법론을 다듬고 논리를 견고히 하는 과정에서는 근거 없이 낯선 주장을 던지는 일이 큰 도움이 되지 않을 것이다.

그러나 기술과 문제의 성격이 빠르게 바뀌는 시기에는 새로운 연구에 배타적인 태도가 큰 문제가 된다.
AI의 비약적인 발전으로 소프트웨어와 하드웨어 모두가 빠르게 변하고 있다.
소프트웨어 개발 방법이 크게 바뀌었고, AI를 위한 하드웨어 설계와 그에 맞는 컴파일러 개발 방법론도 잇달아 나오고 있다.
이런 변화 속에서 과거의 가치만을 내세워 새로운 연구를 배척하는 태도는 학회의 성장에 그다지 도움이 되지 않을 것이다.

이 비판에 대한 개인적인 생각을 덧붙이자면, PLDI도 다소 관대해질 필요가 있지 않을까 한다.
PLDI는 상당히 보수적인 학회로 보인다.
가장 큰 이유는 어떤 현상에 대해서도 이론적으로 타당하고 수학적으로 증명 가능한 설명을 요구하기 때문이다.
이 때문에 성능이 좋은 방법론이 발견되더라도 설명이 충분하지 않으면 배척된다.
아름다운 이론도 좋지만, 현실과 동떨어진 가정 위에 세워진 이론이라면 단지 아름다운 예술 작품에 불과할 것이다.

이와 대조적으로 AI 분야는 이론적 설명을 잠시 제쳐 두고, 우선 실험적으로 효과가 입증된 방법론이 이끄는 형태다.
한 번 실험적 효과가 입증되면, 이론에 집중하는 연구팀이 그 현상에 대한 이론적 설명을 제시하는 방식이 주를 이룬다.
그런 점에서 AI 분야는 PLDI와 달리 개방적이라고 할 수 있지만, 이론적 설명이 부족하면 언젠가 한계에 부딪힌다.
실제로 최근 AI 분야는 과도하게 실험에 치중되어 최신 모델 훈련 방법에 대한 이론적 설명이 매우 부족한 상태다.

흥미롭게도 지난주 열린 ICML에서 Mark Schmidt 교수님이 진행한 튜토리얼에서 방향성에 대한 힌트를 얻을 수 있었다<sup>[4](#mark-schmidt)</sup>.
이론 중심의 연구자들에게는 현재 AI에서 이론이 외면받는 이유가 확장성이 떨어지고, 현실과 동떨어진 가정 아래에서 이론을 제시하기 때문이라는 비판이 있었다.
반대로 실험 중심의 연구자들에게는 무작정 시도해 보고 잘되기를 기대하는 방식으로 연구하지 말고, 이론적 근거를 토대로 체계적인 실험을 하라는 요구가 있었다.
결국 세상의 많은 문제가 그러하듯 적정선을 지키는 일이 중요하다.
PLDI도 이론과 실증의 경계에서 PL의 핵심 가치를 지키는 동시에 새로운 기술에 대한 주도권을 잃지 않기를 바란다.

## PLDI를 떠나며

<table>
  <thead>
    <tr>
      <th style="text-align: center;"><img src="https://lh3.googleusercontent.com/pw/AP1GczOngMZAqJjaTqk3mqYrHA-HjZoq11VtoOuhbIHPFOa9boQYVCI5pWmmPeKkXr2_qXb5ob_3DvTb3yelDj5kcau5bjtn2pl4bre9UPxSIyaPOyMhqF5Gelg8KKoudqr01wMRXyGZhNIYhj6qL9yluYL8=w1078-h1436-s-no-gm"/></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center"><b>학회 마지막 날 찍은 인증 사진</b></td>
    </tr>
  </tbody>
</table>

이번 PLDI에서는 작년과 달리 내 논문도 출판했고, 네트워킹도 훨씬 수월했다.
Expecto 발표 날 외에도, 점심시간에 Shuvendu Lahiri를 직접 찾아가 내 연구에 대한 조언을 들으며 함께 식사했다.
비슷한 연차의 친구들을 만나 내 발표에 초대하고, 연구와 졸업 이후 진로에 관한 고민도 나누었다.
1년 사이에 많은 발전을 이룬 나에게 박수를 보낸다.

그럼에도 아쉬움은 남는다.
발표에서 지나치게 긴장했고, 교수님들이나 회사 사람들과 충분히 네트워킹하지 못했다.
앞으로도 연구와 영어 공부를 게을리하지 않아야겠다는 생각이 든다.

지금 당장은 AI의 눈부신 발전으로 PL과 SE 분야가 조연으로 밀려난 듯하다.
다소 아쉬운 마음이 들지만, AI 에이전트라는 새로운 소프트웨어는 오히려 기존 소프트웨어의 영역을 크게 확장하고, PL이 닿을 수 있는 범위도 넓혀 줄 것이다.
앞으로 AI와 결합한 PL의 엄밀함은 AI를 실제 세상에 적용하는 데 자리한 여러 병목을 해결하는 핵심 열쇠가 될 것이라 믿는다.
그 여정에서 내 연구도 중요한 역할을 할 수 있기를 바란다.

마지막으로 Expecto 연구를 진행하는 데 가장 큰 도움을 주신 교수님께 감사 인사를 드리고 싶다.
연구와 논문에 아낌없이 피드백을 준 연구실 동료들에게도 감사의 말을 전한다.

## 참고 문헌

[<a name="autoverus">1</a>] Chenyuan Yang et al. "[AutoVerus: Automated Proof Generation for Rust Code](https://dl.acm.org/doi/10.1145/3763174)" PACMPL (OOPSLA 2025) \\
[<a name="saman-amarasinghe">2</a>] Saman Amarasinghe. "[Programming Language Design and Implementation for the Machine Learning Era: A Personal Perspective](https://pldi26.sigplan.org/details/pldi-2026-papers/1/Title-TBD)" PLDI Keynote (2026) \\
[<a name="miryung-kim">3</a>] Miryung Kim. "[Happiness U-Curve: Navigating the AI Validation Bottleneck with Conformance Testing and Proof-Engineering](https://pldi26.sigplan.org/details/pldi-2026-papers/2/Hardening-the-Foundation-Testing-Data-and-Compute-Intensive-AI-Enabling-Stacks)" PLDI Keynote (2026) \\
[<a name="mark-schmidt">4</a>] Mark Schmidt. "[Is numerical optimization theory irrelevant to machine learning practice in 2026?](https://blog.icml.cc/2026/04/02/announcing-the-icml-2026-tutorials/)" ICML Tutorial (2026) \\
[<a name="expecto">5</a>] Dongjae Lee and Kihong Heo. "[Expecto: Extracting Formal Specifications from Natural Language Description for Trustworthy Oracles](https://dl.acm.org/doi/10.1145/3808332)" PACMPL (PLDI 2026)
