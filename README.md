# 🎱 로또
로또 게임을 구현한 미션입니다.

## 🎯 구현 순서

### 1️⃣ 구입 금액 입력 및 로또 생성
- [ ] 사용자로부터 구입 금액 입력 받기
  - 1,000원 단위로만 입력 가능
  - 0원 이하 입력 불가
  - 숫자가 아닌 값 입력 불가
- [ ] 입력받은 금액에 따른 로또 발급
  - 1장당 1,000원
  - 각 로또는 1~45 사이의 서로 다른 숫자 6개로 구성
  - 오름차순 정렬하여 표시

### 2️⃣ 당첨 번호 입력
- [ ] 당첨 번호 6개 입력 받기
  - 쉼표(,)로 구분된 숫자 입력
  - 숫자는 1~45 범위여야 함
  - 중복된 숫자 입력 불가
  - 정확히 6개의 숫자만 입력
  - 숫자가 아닌 값 입력 불가
- [ ] 보너스 번호 1개 입력 받기
  - 1~45 범위의 숫자
  - 기존 당첨 번호와 중복 불가
  - 숫자가 아닌 값 입력 불가

### 3️⃣ 당첨 결과 계산
- [ ] 당첨 여부 확인
  - 구매한 각 로또와 당첨 번호 비교
  - 일치하는 번호 개수 확인
  - 보너스 번호 일치 여부 확인
- [ ] 당첨 통계 생성
  - 3개 일치 (5등, 5,000원)
  - 4개 일치 (4등, 50,000원)
  - 5개 일치 (3등, 1,500,000원)
  - 5개 + 보너스 번호 일치 (2등, 30,000,000원)
  - 6개 일치 (1등, 2,000,000,000원)

### 4️⃣ 결과 출력
- [ ] 구매 내역 출력
  - 구입한 로또 수량 표시
  - 각 로또 번호 출력 (오름차순)
- [ ] 당첨 통계 출력
  - 당첨 등수별 개수 표시
  - 당첨금액 표시
- [ ] 수익률 출력
  - (당첨 금액 총합 / 구매 금액) × 100
  - 소수점 둘째 자리에서 반올림

## 🚨 예외 상황
- [ ] 모든 예외 상황에서 "[ERROR]"로 시작하는 메시지 출력
- [ ] 예외 발생 시 해당 부분부터 입력 다시 받기
- [ ] 각 단계별 유효성 검증
  - 금액 검증
  - 로또 번호 범위 검증
  - 중복 번호 검증
  - 입력 형식 검증

## 💻 프로그래밍 요구사항
- JDK 21 사용
- 클래스 구조 준수 (상수 → 멤버변수 → 생성자 → 메서드)
- indent depth 2까지만 허용
- 메서드 길이 15라인 제한
- else 키워드 사용 금지
- 모든 기능은 단위 테스트 작성