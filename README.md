# javascript-lotto-precourse

# 기능 목록

## 입력

- [x] 1,000원 단위로 로또 구입 금액을 입력받는다.
  - [ ] 잘못된 값을 입력할 경우 "[ERROR]"로 시작하는 메시지와 함께 `Error`를 발생시킨다. 잘못된 값은 아래에 해당한다.
    - [x] 1,000원으로 나누어 떨어지지 않는 경우 = 1,000원 미만인 경우
    - [x] 입력값이 숫자가 아닌 경우
  - [x] 에러 발생 후, 해당 지점부터 다시 입력받는다.
- [x] 로또발행 내역이 출력된 후, 쉼표(,)를 기준으로 6개의 당첨 번호를 입력받는다.
  - [ ] 예외처리 `Error` 예외의 경우는 밑에 해당한다.
    - [ ] 1~45 사이의 숫자가 아닌 경우
- [x] 당첨번호 입력받은 후, 보너스 번호를 입력받는다.
  - [ ] 예외처리 `Error`
    - [ ] 1~45 사이의 숫자가 아닌 경우

## 출력

- [x] 발행한 로또 수량을 출력한다.
- [x] 오름차순 정렬된 로또 번호들을 로또 수량만큼 출력한다.
- [ ] 계산되어 반환된 당첨내역을 출력한다.
- [ ] 계산되어 반환된 수익률을 출력한다.

## 핵심 기능

- [x] 입력받은 로또 구입 금액에 해당하는 만큼 로또를 발행한다. (로또 1장은 1,000원이다)
  - [x] 로또 1장 당 1~45 사이의 중복되지 않는 6개의 숫자를 뽑는다.
  - [x] 숫자들을 오름차순 정렬한다.
- [x] 입력받은 당첨 번호 문자열을 구분자(,)를 기준으로 배열에 저장한다.
- [x] 구분자로 분리된 당첨 번호 문자열 배열을 숫자형으로 변환한다.
- [ ] 사용자가 구매한 로또 번호와, 당첨 번호를 비교해 당첨내역을 계산해 반환한다.

  - [x] 점수를 계산한다.

    - [x] 1등: 6개 번호 일치(6점)
    - [x] 2등: 5개 번호(5점) + 보너스 번호 일치(true)
    - [x] 3등: 5개 번호 일치(5점)
    - [x] 4등: 4개 번호 일치(4점)
    - [x] 5등: 3개 번호 일치(3점)
- [ ] 소수점 둘째 자리에서 반올림 한 수익률을 계산해 반환한다.
