# 노벨피아 인디케이터

노벨피아 작품의 회차별 조회수·추천수, 연독률, 급락 밴드, 안정성 점수 및 종합 등급을 분석하는 Violentmonkey 사용자 스크립트입니다.

## 설치

[![노벨피아 인디케이터 설치](https://img.shields.io/badge/Violentmonkey-원클릭_설치-2563EB?style=for-the-badge&logo=firefoxbrowser&logoColor=white)](https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js)

**Android Firefox + Violentmonkey**를 설치한 뒤 위 버튼을 누르면 사용자 스크립트 설치 확인 화면이 열립니다. 설치 확인을 눌러 완료하세요. (브라우저/확장 기능에 따라 파일이 다운로드되면 Violentmonkey에서 'URL에서 설치'를 이용하세요.) v1.3.6 이하를 기존에 설치했다면 이번 한 번은 기존 스크립트를 제거하거나 새 코드로 교체해야 합니다. 중복 설치를 피하세요.

## 방문 통계

[![README 조회 횟수](https://hits.sh/github.com/theturtle175/novelpia_indicator.svg?style=flat&label=README%20views&color=2563eb)](https://hits.sh/github.com/theturtle175/novelpia_indicator/)

- **README 조회 횟수:** 외부 방문 카운터가 집계한 이미지 요청 수입니다. GitHub 이미지 캐시, 반복 방문 등에 영향을 받으므로 **실제 순 방문자 수나 스크립트 설치 수가 아닙니다.**
- **공식 순 방문자 수:** [GitHub Insights → Traffic](https://github.com/theturtle175/novelpia_indicator/graphs/traffic)에서 최근 14일간의 고유 방문자 수를 확인할 수 있습니다. 해당 통계는 저장소 쓰기 권한이 있는 계정에서 확인 가능합니다.
- 카운터는 추가한 시점부터 집계되며, 과거 방문 횟수는 소급하지 않습니다. 외부 서비스 [hits.sh](https://hits.sh/)를 사용하므로 서비스 상태에 따라 표시되지 않을 수 있습니다.

## 자동 업데이트

v1.3.7부터 GitHub의 공개 배포 파일에 다음 메타데이터를 포함합니다.

- `@updateURL`: `https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js`
- `@downloadURL`: 위와 동일한 주소
- `@version`: 1.3.11

앞으로 새 버전을 게시할 때는 `main/novelpia_indicator.user.js`의 `@version`과 내부 `VERSION`을 함께 올려야 합니다. Violentmonkey의 자동 업데이트 확인 주기 및 환경에 따라 실제 반영 시점은 달라집니다. 필요하면 확장 프로그램에서 수동으로 업데이트를 확인하세요.

GitHub에 코드를 올리기만 해서는 즉시 설치 스크립트가 변경되지 않습니다. 버전이 높아지고 업데이트 확인이 이루어져야 합니다.

## 지원 범위

- 노벨피아 작품별 공개 회차 데이터 분석
- 조회수·추천수, 회차별 그래프, 연독률 및 안정성 평가
- 종합 점수와 9등급 캐릭터
- Android Firefox + Violentmonkey 대상으로 개발

**최신 버전: v1.3.11.** 날짜만 표시된 회차는 공개일로부터 3일 뒤 0시(KST)부터 평가에 포함하고, 최신 3개 회차는 항상 제외합니다. 정확한 공개 시각을 확인할 수 있는 경우에는 공개 후 72시간을 적용합니다. 평균 조회수·추천률·장기 연독률·안정성 점수에 같은 제외 기준을 적용하되 전체 누적 조회수는 모든 회차를 표시합니다. GitHub 자동 업데이트 기능은 유지합니다.
