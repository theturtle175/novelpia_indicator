# 노벨피아 인디케이터

노벨피아 작품의 회차별 조회수·추천수, 연독률, 급락 밴드, 안정성 점수 및 종합 등급을 분석하는 Violentmonkey 사용자 스크립트입니다.

## 설치

[![노벨피아 인디케이터 설치](https://img.shields.io/badge/Violentmonkey-원클릭_설치-2563EB?style=for-the-badge&logo=firefoxbrowser&logoColor=white)](https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js)

**Android Firefox + Violentmonkey**를 설치한 뒤 위 버튼을 누르면 사용자 스크립트 설치 확인 화면이 열립니다. 설치 확인을 눌러 완료하세요. (브라우저/확장 기능에 따라 파일이 다운로드되면 Violentmonkey에서 'URL에서 설치'를 이용하세요.) v1.3.6 이하를 기존에 설치했다면 이번 한 번은 기존 스크립트를 제거하거나 새 코드로 교체해야 합니다. 중복 설치를 피하세요.

## Greasy Fork 배포 및 설치 통계

[![Greasy Fork 게시 설정](https://img.shields.io/badge/Greasy%20Fork-설치%20통계%20연결%20안내-229954?style=for-the-badge)](./docs/GREASY_FORK_SETUP.md)

Greasy Fork는 **설치 횟수·일별 설치·업데이트 확인 횟수**를 집계합니다. GitHub `main`의 원본 스크립트를 가져와 **자동 동기화**할 수 있습니다.

> **현재 상태: 게시자 계정으로 Greasy Fork 최초 등록 전.** 통계 수집은 그 사이트에 실제로 게시되어 Greasy Fork 설치 버튼을 사용하기 시작한 후부터 가능합니다. 기존 GitHub Raw 설치 수는 소급 집계되지 않습니다.

- [Greasy Fork 등록 페이지(로그인 필요)](https://greasyfork.org/ko/import)
- [등록·자동 동기화·설치 통계 상세 안내](./docs/GREASY_FORK_SETUP.md)
- 등록할 GitHub raw 주소: `https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js`

Greasy Fork에 실제 게시한 뒤에는 위의 **GitHub 직접 설치 버튼** 대신 **Greasy Fork 배포 페이지의 설치 버튼**을 주된 설치 경로로 안내해야 통계가 집계됩니다. 기존 GitHub 자동 업데이트는 유지합니다.

## 자동 업데이트

v1.3.7부터 GitHub의 공개 배포 파일에 다음 메타데이터를 포함합니다.

- `@updateURL`: `https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js`
- `@downloadURL`: 위와 동일한 주소
- `@version`: 1.3.9

앞으로 새 버전을 게시할 때는 `main/novelpia_indicator.user.js`의 `@version`과 내부 `VERSION`을 함께 올려야 합니다. Violentmonkey의 자동 업데이트 확인 주기 및 환경에 따라 실제 반영 시점은 달라집니다. 필요하면 확장 프로그램에서 수동으로 업데이트를 확인하세요.

GitHub에 코드를 올리기만 해서는 즉시 설치 스크립트가 변경되지 않습니다. 버전이 높아지고 업데이트 확인이 이루어져야 합니다.

## 지원 범위

- 노벨피아 작품별 공개 회차 데이터 분석
- 조회수·추천수, 회차별 그래프, 연독률 및 안정성 평가
- 종합 점수와 9등급 캐릭터
- Android Firefox + Violentmonkey 대상으로 개발

**최신 버전: v1.3.9.** 만료된 분석 체크포인트를 안전하게 정리하고, 브라우저 저장 용량 초과 시 오래된 완료 기록 삭제 후 재시도합니다. 저장 오류 원인을 구분해서 표시하며 기존 분석 계산식과 GitHub 자동 업데이트 기능은 유지합니다.
