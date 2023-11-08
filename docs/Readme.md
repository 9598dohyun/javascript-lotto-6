## 요구사항 목록
1. 로또 번호 생성:
   - 로또 번호는 1부터 45까지의 중복되지 않는 숫자 6개를 생성합니다.
   - 사용자가 로또금액을 입력하면 금액만큼 로또번호를 생성한다. 이때 장당 가격은 1000원이다.
   
2. 당첨 번호 추첨:
   - 당첨 번호는 1부터 45까지의 숫자이며 중복되지 않는 숫자 6개와 보너스번호를 사용자가 입력한다. 구분은 쉼표로 한다.
   
3. 당첨 결과 계산 및 출력:
    ```
    - 발행된 로또 번호와 당첨 번호를 비교하여 각 등수별 당첨 여부를 확인하고, 당첨 금액을 계산합니다.
    - 당첨 등수는 다음과 같습니다:
        - 5등: 3개 번호 일치 / 5,000원
        - 4등: 4개 번호 일치 / 50,000원
        - 3등: 5개 번호 일치 / 1,500,000원
        - 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
        - 1등: 6개 번호 일치 / 2,000,000,000원
    - 수익률을 계산한다.
        - 수익률은 둘째자리에서 반올림한다.
    ```
4. 예외 처리:

    - 사용자가 잘못된 값을 입력할 경우 예외처리를 하고 다시 입력하도록 합니다.

5. 입출력 요구사항:
    1. 로또 구입 금액, 당첨 번호, 보너스 번호 순으로 입력받습니다.
    2. 발행한 로또 번호와 당첨 결과를 출력합니다.
    3. 수익률을 계산하여 출력합니다.

6. 리팩토링:
    - 함수 분리 및 재사용성 증대하도록 수정합니다.
    - 함수(또는 메서드)의 길이가 15라인을 넘어가지 않도록 구현한다.
    - else를 지양한다.
    - indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
    - 상수 관리를 해줍니다.