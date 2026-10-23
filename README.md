# 노벨피아 인디케이터

노벨피아 작품의 회차별 조회수·추천수, 연독률, 급락 밴드, 안정성 점수 및 종합 등급을 분석하는 Violentmonkey 사용자 스크립트입니다.

## 설치

**[최신 버전 설치 (.user.js)](https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js)**

Android Firefox + Violentmonkey에서 위 링크를 열어 설치하세요. v1.3.6 이하를 기존에 설치했다면 이번 한 번은 기존 스크립트를 제거하거나 새 코드로 교체해야 합니다. 중복 설치를 피하세요.

## 자동 업데이트

v1.3.7부터 GitHub의 공개 배포 파일에 다음 메타데이터를 포함합니다.

- `@updateURL`: `https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js`
- `@downloadURL`: 위와 동일한 주소
- `@version`: 1.3.7

앞으로 새 버전을 게시할 때는 `main/novelpia_indicator.user.js`의 `@version`과 내부 `VERSION`을 함께 올려야 합니다. Violentmonkey의 자동 업데이트 확인 주기 및 환경에 따라 실제 반영 시점은 달라집니다. 필요하면 확장 프로그램에서 수동으로 업데이트를 확인하세요.

GitHub에 코드를 올리기만 해서는 즉시 설치 스크립트가 변경되지 않습니다. 버전이 높아지고 업데이트 확인이 이루어져야 합니다.

## 지원 범위

- 노벨피아 작품별 공개 회차 데이터 분석
- 조회수·추천수, 회차별 그래프, 연독률 및 안정성 평가
- 종합 점수와 9등급 캐릭터
- Android Firefox + Violentmonkey 대상으로 개발

v1.3.7은 v1.3.6에 자동 업데이트용 메타데이터를 추가한 릴리스이며 기존 분석 계산식은 유지합니다.
