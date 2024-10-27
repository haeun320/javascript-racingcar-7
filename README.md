<p align="center">
  <img src="https://i.ibb.co/D1CHbsB/logo-dark.png" width=300 alt="우아한프리코스"/>
</p>

# 프리코스 2주차 - 자동차 경주

### 목차

[🛠️ 기능 목록](#️-기능-목록) &nbsp;
[✏️ 추가 정의 사항](#️-추가-정의-사항) &nbsp;
[⚠️ 에러 상황](#️-에러-상황) &nbsp;
[🖥️ 입출력 예시](#️-입출력-예시)

<br/>

## 🛠️ 기능 목록

1. 경주할 자동차 이름을 입력받는다. 이름은 쉼표를 기준으로 구분하며, 5자 이하로 제한된다.

2. 시도할 횟수를 입력받는다.
3. 자동차 이름, 시도 횟수 입력에서 잘못된 값이 입력되면 [ERROR]로 시작하는 메시지와 함께 Error를 발생시킨 후 종료된다.
4. 입력받은 횟수 동안 각 자동차는 전진 또는 멈출 수 있다.<br/>- 0~9 사이의 랜덤한 값이 4인 경우 전진한다.
5. 매 횟수의 실행 결과를 출력한다. 자동차 출력은 입력 받은 순서대로 출력한다.
6. 입력받은 횟수의 자동차 경주가 완료되면, 가장 많이 전진한 자동차를 우승자로 출력한다.
7. 우승자는 한 명 이상일 수 있다. 우승자가 여러명인 경우 쉼표를 기준으로 구분한다. 출력 순서는 입력 받은 순서이다.

<br/>

## ✏️ 추가 정의 사항

1. 자동차 이름은 1자 이상 5자 이하의 문자열이며, 공백을 허용한다. 단, 공백 문자만을 입력할 수는 없다.

2. 경주할 자동차는 1개 이상이다.
3. 시도할 횟수는 양의 정수이다.
4. 최대 시도 횟수는 100회로 제한한다.

<br/>

## ⚠️ 에러 상황

1. 쉼표로 구분된 자동차 이름이 6글자 이상일 때

2. 자동차 이름으로 공백 문자만을 입력할 때
3. 입력된 자동차가 0개일 때<br/>- 아무것도 입력하지 않고 엔터 입력<br/>- 공백 문자만 입력하고 엔터 입력
4. 시도할 횟수로 양의 정수가 아닌 입력을 할 때
5. 시도할 횟수로 100 이상의 수를 입력할 때
6. 시도할 횟수를 입력하지 않을 때

<br/>

## 🖥️ 입출력 예시

```
경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)
pobi,woni,jun
시도할 횟수는 몇 회인가요?
5

실행 결과
pobi : -
woni :
jun : -

pobi : --
woni : -
jun : --

pobi : ---
woni : --
jun : ---

pobi : ----
woni : ---
jun : ----

pobi : -----
woni : ----
jun : -----

최종 우승자 : pobi, jun
```