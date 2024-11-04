# java-lotto-precourse

### 0. 게임 진행 문구를 출력하는 기능

- [x] 0.1 구입금액 입력 안내 문구를 출력한다.
- [x] 0.2 구매한 로또 수량 및 번호를 출력한다. (번호는 오름차순 정렬)
- [x] 0.3 당첨 번호 입력 안내 문구를 출력한다.
- [x] 0.4 보너스 번호 입력 안내 문구를 출력한다.
- [x] 0.5 당첨 통계 결과를 출력한다.

### 1. 입력을 받는 기능

- [x] 1.1 구입 금액을 입력받는다.
- [x] 1.2 구입 금액이 1,000원으로 나누어 떨어지는지 검증한다.
- [x] 1.3 당첨 번호를 입력받는다. (쉼표로 구분된 6개의 숫자)
- [x] 1.4 당첨 번호가 1부터 45 사이의 숫자인지 검증한다.
- [x] 1.5 당첨 번호에 중복된 숫자가 없는지 검증한다.
- [x] 1.6 보너스 번호를 입력받는다.
- [x] 1.7 보너스 번호가 1부터 45 사이의 숫자인지 검증한다.
- [x] 1.8 보너스 번호가 당첨 번호와 중복되지 않는지 검증한다.

### 2. 로또 번호 생성 기능

- [x] 2.1 구매한 수량만큼 로또 번호를 생성한다.
- [x] 2.2 로또 번호는 1부터 45 사이의 중복되지 않는 6개의 숫자로 구성된다.
- [x] 2.3 로또 번호를 오름차순으로 정렬한다.

### 3. 당첨 결과 계산 기능

- [x] 3.1 구매한 각 로또 번호와 당첨 번호를 비교하여 일치하는 숫자 개수를 계산한다.
- [x] 3.2 보너스 번호 일치 여부를 확인한다.
- [x] 3.3 일치하는 숫자 개수 및 보너스 번호 일치 여부로 당첨 등수를 판단한다.
- [x] 3.4 당첨 등수별로 당첨 횟수를 누적한다.
- [x] 3.5 총 당첨 금액을 계산한다.

### 4. 결과를 출력하는 기능

- [x] 4.1 당첨 통계를 출력한다. (등수별 당첨 횟수)
- [x] 4.2 총 수익률을 계산하여 소수점 둘째 자리에서 반올림한다.
- [x] 4.3 총 수익률을 출력한다.

### 5. 예외 상황 처리

- [x] 5.1 사용자가 입력한 값이 빈 문자열인 경우 예외 처리한다.
- [x] 5.2 구입 금액이 1,000원 단위가 아닌 경우 예외 처리한다.
- [x] 5.3 구입 금액 입력에 숫자가 아닌 값이 포함된 경우 예외 처리한다.
- [x] 5.4 당첨 번호 입력 시 숫자가 아닌 값이 포함된 경우 예외 처리한다.
- [x] 5.5 당첨 번호가 6개가 아닌 경우 예외 처리한다.
- [x] 5.6 당첨 번호에 중복된 숫자가 있는 경우 예외 처리한다.
- [x] 5.7 당첨 번호가 1부터 45 사이의 숫자가 아닌 경우 예외 처리한다.
- [x] 5.8 보너스 번호가 숫자가 아닌 경우 예외 처리한다.
- [x] 5.9 보너스 번호가 1부터 45 사이의 숫자가 아닌 경우 예외 처리한다.
- [x] 5.10 보너스 번호가 당첨 번호와 중복되는 경우 예외 처리한다.
- [x] 5.11 예외 발생 시 "[ERROR]"로 시작하는 에러 메시지를 출력한다.

### 6. 기타 요구 사항

- [x] 6.1 Lotto 클래스를 사용하여 로또 번호를 관리한다.
- [x] 6.2 Lotto 클래스의 numbers 이외의 필드를 추가하지 않는다.
- [x] 6.3 Lotto 클래스의 numbers 필드의 접근 제어자인 private을 변경하지 않는다.

### 7. 클래스별 역할

    1. Lotto: 로또 번호의 생성과 validation 검사, 번호 일치 개수 및 보너스 번호 일치 여부를 판단합니다.
    2. WinningNumbers: 당첨 번호를 관리
    3. BonusNumber: 보너스 번호를 관리
    4. LottoGenerator: 로또 구매와 관련된 기능을 담당하며 구매한 로또 리스트를 관리합니다.
    5. InputView: 사용자 입력과 관련된 기능을 담당하며 입력된 값을 저장하고 제공합니다.
    6. Result: 당첨 결과의 계산과 출력을 담당하며 결과 데이터를 관리합니다.
    7. LottoGame: 게임의 전체적인 흐름을 제어하며 각 객체를 생성하고 협력하여 프로그램을 실행합니다.