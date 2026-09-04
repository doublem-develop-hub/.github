# 🔒 DoubleM Develop Hub

**DoubleM Social Company** 개발팀의 내부 개발 조직입니다.

서비스 개발, 정부지원사업, 연구개발 및 사내 프로젝트의 소스 코드와 기술 자산을 관리합니다.



## 📁 Repository Structure

프로젝트 Repository는 아래 규칙을 기준으로 관리합니다.

### Project Type

| Prefix | Description |
|--------|-------------|
| `gov` | 정부지원사업 및 공공 프로젝트 |
| `svc` | 자사 서비스 및 외부 서비스 |
| `int` | 사내 시스템 및 내부 도구 |
| `rnd` | 연구개발 및 기술 검증 |

### Naming Convention

`{type}-{project}-{year}`

Example:

- `gov-dex-2026`
- `svc-project-name-2026`
- `int-project-name-2026`
- `rnd-project-name-2026`

프로젝트 규모에 따라 Repository를 역할별로 분리합니다.

- `gov-dex-2026-api`
- `gov-dex-2026-web`
- `gov-dex-2026-admin`
- `gov-dex-2026-infra`



## 🌿 Branch Strategy

- `main` — Production
- `develop` — Development
- `feature/*` — Feature Development
- `fix/*` — Bug Fix
- `hotfix/*` — Production Hotfix

모든 변경사항은 Pull Request를 통해 병합하는 것을 원칙으로 합니다.



## 📝 Commit Convention

- `feat:` 새로운 기능
- `fix:` 버그 수정
- `refactor:` 코드 리팩토링
- `docs:` 문서 수정
- `test:` 테스트 코드
- `chore:` 설정 및 기타 작업

Example:

`feat: 사용자 인증 API 구현`  
`fix: 로그인 토큰 갱신 오류 수정`  
`refactor: 인증 서비스 구조 개선`



## 🔐 Security

- Repository는 기본적으로 `Private`으로 관리합니다.
- API Key, Secret Key, 인증서 등 민감정보를 Repository에 포함하지 않습니다.
- 환경변수는 `.env` 또는 별도의 Secret Manager를 사용합니다.
- 프로젝트 접근 권한은 최소 권한 원칙을 적용합니다.
