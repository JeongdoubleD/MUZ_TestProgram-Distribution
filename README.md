# MUZ_TestProgram Distribution

MUZ_TestProgram의 설치파일 배포 및 업데이트 확인용 저장소입니다. 소스코드는 포함하지 않으며, 빌드된 설치파일과 버전 매니페스트만 관리합니다.

## 파일

- `customer-latest.json` — 고객사 배포 채널 최신 버전 정보 (Release 빌드가 확인)
- `internal-latest.json` — 사내 배포 채널 최신 버전 정보 (ReleaseInternal 빌드가 확인, 내부 도구 포함 버전)

## 릴리스 태그 규칙

- 고객사용: `customer-v{version}` (예: `customer-v1.2.60`)
- 사내용: `internal-v{version}` (예: `internal-v1.2.60`)

각 릴리스에 `MUZ_TestProgram_Setup.exe` 설치파일을 첨부하고, 대응하는 `*-latest.json`의 `version`/`url`을 갱신합니다.

고객사 채널은 검증이 끝난 버전만 갱신하고, 사내 채널은 패치마다 자주 갱신합니다.
