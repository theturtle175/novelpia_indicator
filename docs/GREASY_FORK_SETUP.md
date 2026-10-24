# Greasy Fork 배포·설치 통계 연결 안내

## 현황

- GitHub 정식 소스: [novelpia_indicator.user.js](../novelpia_indicator.user.js)
- GitHub 자동 업데이트: 유지 (`@version` / `@updateURL` / `@downloadURL`)
- Greasy Fork **최초 게시: 계정 소유자 승인 전**, 아직 배포 페이지 URL 없음
- 코드 변경: 없음. 별도 추적 코드·방문자 식별 기능을 삽입하지 않음.

## 1. Greasy Fork에서 최초 게시

1. [Greasy Fork 로그인](https://greasyfork.org/ko)에 본인의 계정으로 로그인합니다.
2. [외부 스크립트 가져오기](https://greasyfork.org/ko/import)를 엽니다.
3. 아래 **원본 주소**를 입력합니다. 반드시 GitHub `main` 브랜치를 가리키는 raw 파일 주소여야 합니다.

   ```text
   https://raw.githubusercontent.com/theturtle175/novelpia_indicator/main/novelpia_indicator.user.js
   ```

4. **동기화 방식: 자동(Automatically / periodically update it from the URL)**을 선택합니다.
5. 스크립트 이름·한국어 설명·적용 사이트(`novelpia.com`)·버전 및 코드 내용을 확인하고 게시합니다.
6. 첫 게시 후 관리 화면에서 마지막 동기화 시각·오류 여부를 확인합니다.

> 반드시 본인의 Greasy Fork 로그인으로 게시를 승인해야 합니다. 이 저장소만 변경해서는 Greasy Fork의 계정이나 배포 페이지가 생기지 않습니다.

## 2. 이후 버전 관리

- GitHub `main/novelpia_indicator.user.js`를 단일 원본으로 유지합니다.
- 릴리스마다 사용자 스크립트의 `@version`과 내부 `VERSION`을 함께 증가시킵니다.
- Greasy Fork 자동 동기화 설정이 해당 raw 주소를 읽어 새 버전을 게시하도록 합니다.
- GitHub에서 설치한 사용자들은 기존 GitHub 업데이트 경로를 이용합니다.
- **Greasy Fork를 통해 설치한 사용자들**은 Greasy Fork가 제공하는 설치 코드의 `@updateURL` / `@downloadURL`에 따라 해당 플랫폼을 통해 업데이트됩니다.
- Greasy Fork는 게시 스크립트의 메타데이터에 있는 업데이트/다운로드 주소를 Greasy Fork 주소로 재작성하므로, GitHub 코드의 원본 주소를 일부러 바꿀 필요가 없습니다.
- 동기화가 실패하면 Greasy Fork 관리 화면에서 오류 및 크기 제한, 유효한 사용자 스크립트 형식, 외부 코드 정책을 확인합니다.

## 3. 설치 통계

Greasy Fork의 해당 스크립트 페이지에서 **통계(Stats)** 탭을 열면 다음 지표를 확인할 수 있습니다.

| 항목 | 의미 |
| --- | --- |
| Total installs | Greasy Fork를 통한 누적 설치 버튼 클릭 집계 |
| Daily installs | 일별 설치 집계 |
| Update checks | 사용자 스크립트 매니저가 Greasy Fork에 업데이트를 확인한 횟수 |

- **과거 GitHub Raw 직접 설치나 파일 공유 내역은 소급 집계되지 않습니다.**
- 설치 수는 정확한 고유 사용자·활성 사용자 수가 아니며, 재설치 등이 포함될 수 있습니다.
- Github README의 현재 설치 버튼은 GitHub raw를 가리킵니다. Greasy Fork 설치 통계에 포함시키려면 **Greasy Fork 게시가 완료된 후** 실제 Greasy Fork 배포 페이지의 녹색 설치 버튼으로 안내 링크를 변경해야 합니다.
- Greasy Fork에 게시한 뒤 **실제 배포 페이지 주소**를 알려주면 README에 Greasy Fork 설치 버튼과 통계 페이지 링크를 연결할 수 있습니다.

## 4. 유의 사항

- Greasy Fork의 일반 사용자 스크립트 크기 제한은 2MB입니다. 현재 코드에는 사용자가 제공한 등급 이미지 데이터가 포함되어 있으므로 게시 시 제한을 확인합니다.
- Greasy Fork가 게시한 스크립트의 코드를 검토할 수 있도록 코드를 외부 로더 형태로 대체하지 않습니다.
- 등급 이미지·코드의 재배포 권리와 라이선스는 소유자가 확인해야 합니다. 임의로 라이선스를 부여하지 않습니다.
- 이미 설치한 동일 스크립트를 중복 설치하지 않도록 배포 페이지에서 안내합니다.

[Greasy Fork 공식 코드 규칙](https://greasyfork.org/ko/help/code-rules) · [Greasy Fork 메타데이터 재작성 정책](https://greasyfork.org/ko/help/rewriting) · [Greasy Fork API와 동기화](https://greasyfork.org/ko/help/api)
