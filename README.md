# 권태근 포트폴리오

토목산업기사 필기 합격과 실무 결과물을 카테고리별로 정리한 저장소입니다.

**보기: https://kwontaegeun.vercel.app**

이 저장소 맨 위의 `index.html`이 포트폴리오 페이지입니다. main이 바뀌면 Vercel이 자동으로 다시 배포합니다.

## 카테고리

| 폴더 | 분야 | 담긴 것 |
|---|---|---|
| [01-certificates](01-certificates/) | 자격·수료 | 토목산업기사(필기 합격 · 최종 발표 2026.12.18), AI 윤리 수료증 |
| [02-structural-design](02-structural-design/) | 구조 설계 · 시공 계획 | 스파게티 교량: 처음 3D 설계, 18단계 시공 순서 시뮬레이션 |
| [03-safety-diagnosis](03-safety-diagnosis/) | 유지관리 · 안전진단 | 청계천복개(좌안) 정밀안전진단 보고서 분석 |
| [04-data-analysis](04-data-analysis/) | 사업 분석 · 데이터 자동화 | 현대건설 10년 재무제표 분석과 자동 대시보드 |

## 파일 구조

```
index.html                         포트폴리오 페이지
01-certificates/
  coursera-ai-ethics-certificate.pdf   AI 윤리 수료증
02-structural-design/
  first-3d-design.html                 처음 3D 설계
  construction-sequence-simulation.html  18단계 시공 순서 시뮬레이션
  images/                              포트폴리오에 쓴 그림 5장
03-safety-diagnosis/                   보고서 분석 설명
04-data-analysis/
  images/                              대시보드 그림
```

각 폴더의 README에 자세한 설명과 바로 열 수 있는 주소가 있습니다.

## 배포 (Vercel)

| 항목 | 설정 |
|---|---|
| 공개 주소 | https://kwontaegeun.vercel.app |
| Vercel 프로젝트 | `kwontaegeun` (kwontk2006-ai 계정, Hobby) |
| 연결 저장소 · 브랜치 | `HSC-Class01/KTG_portforlio` · `main` |
| 빌드 | Root Directory 비움(저장소 맨 위) · Framework Preset `Other` · 빌드 명령 없음 (파일을 그대로 올림) |
| 자동 배포 | `main`에 푸시하면 다시 배포되고, 커밋 옆에 Vercel 배포 상태가 표시됨 |

### 권한 설정

배포에는 아래 두 가지 연결이 필요하고, 둘 다 설정되어 있습니다.

| 어디에서 | 무엇을 | 현재 상태 |
|---|---|---|
| GitHub 조직 `HSC-Class01` → Settings → GitHub Apps → Vercel → Configure → Repository access | Vercel 앱이 읽을 수 있는 저장소 | Only select repositories에 `KTG_portforlio` 포함 |
| Vercel 프로젝트 `kwontaegeun` → Settings → Git | 배포에 연결할 저장소 | `HSC-Class01/KTG_portforlio` 연결 |

- 조직의 GitHub App 설정은 조직 소유자(Owner)만 바꿀 수 있습니다. 소유자가 아니면 같은 화면에서 요청(Request)을 보내 승인을 받습니다.
- Vercel 저장소 목록에 `KTG_portforlio`가 보이지 않으면, 위 GitHub 화면에서 저장소를 추가한 뒤 Vercel의 `Adjust GitHub App Permissions`로 목록을 다시 불러옵니다.

### 공개 범위

Settings → Deployment Protection은 `Vercel Authentication` · `Standard Protection`입니다.

- `kwontaegeun.vercel.app`(실제 주소)은 로그인 없이 열립니다.
- 배포마다 생기는 개별 주소(`kwontaegeun-…-kwontk2006-ai.vercel.app`)는 Vercel 로그인 화면으로 넘어갑니다. 공유할 때는 실제 주소를 씁니다.
