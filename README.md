# 자리 배치 추첨 프로그램

원형으로 자리를 배치하고 랜덤으로 자리를 배정하는 프로그램입니다.

## 주요 기능

* 원형 자리 배치 시각화
* 동적 그룹 크기 조절 (사용자 지정 가능)
* 엑셀 파일에서 이름 목록 불러오기
* 수동으로 이름 입력 가능
* 이전 추첨 결과와 중복되지 않는 새로운 자리 배치
* 결과 저장 및 이력 관리
* 그룹별 색상 구분

## 설치 방법

1. 저장소 클론
```bash
git clone https://github.com/kdc0901/random-number.git
cd random-number
```

2. 필요한 패키지 설치
```bash
pip install -r requirements.txt
```

## 사용 방법

1. 프로그램 실행
```bash
python random_lottery_gui.py
```

2. 이름 입력 방법
   * 직접 입력: 좌측의 입력 필드에 이름을 직접 입력
   * 엑셀 파일 불러오기: "엑셀 파일 불러오기" 버튼 클릭

3. 그룹 설정
   * "그룹 크기" 입력란에 원하는 그룹 크기 입력 (기본값: 6)
   * "그룹으로 묶기" 버튼으로 그룹 표시 켜기/끄기

4. 자리 배치
   * "자리 배치하기" 버튼을 클릭하면 랜덤으로 자리가 배정됩니다
   * 이전 추첨 결과와 중복되지 않는 새로운 배치가 생성됩니다

## 주의사항

* 엑셀 파일 형식: 두 번째 열(B열)에 이름이 있어야 합니다
* 최대 43명까지 자리 배치 가능
* `lottery_history.json` 파일에 이전 추첨 결과가 저장됩니다 