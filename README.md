# SBCData — 실험 및 PRD 문서

Seoul Beauty Club의 제품 실험 설계와 PRD(제품 요구사항 문서)를 관리하는 리포지토리입니다.

## 문서 구조

| 경로 | 내용 |
|---|---|
| [docs/planning/2026-W28-product-planning.md](docs/planning/2026-W28-product-planning.md) | **이번 주** 주간 프로덕트 플래닝 초안 (2026 W28, 7/6–7/12) |
| [docs/experiments/00-experiment-overview.md](docs/experiments/00-experiment-overview.md) | 실험 전체 구조, 로드맵, 공통 지표 및 가드레일 |
| [docs/prd/01-free-addon-reward-test.md](docs/prd/01-free-addon-reward-test.md) | **[우선순위 1]** 첫 박스 수령자 대상 첫 리뷰 크레딧 리워드 테스트 PRD (첫 리뷰 작성 → 20크레딧) |
| [docs/prd/02-hybrid-recommendation-discovery.md](docs/prd/02-hybrid-recommendation-discovery.md) | 하이브리드 추천(소셜 × 콘텐츠 × 트렌딩) 및 태그/라벨 실험 PRD |
| [docs/prd/03-review-reward-gamification.md](docs/prd/03-review-reward-gamification.md) | **[E1 후속]** 리뷰 리워드 게이미피케이션 PRD — 포인트 + 배지/레벨, 단계적 론칭 (미국 시장 벤치마크 포함) |

## 배경

세 개의 트랙이 논의되었습니다.

1. **리워드 테스트 (우선 진행)** — 전면적인 보상 체계 도입 전에, 첫 번째 박스 수령자가 첫 리뷰를 작성하면 다음 박스 애드온 구매에 쓸 수 있는 20크레딧($20 가치)을 지급하는 선행 테스트를 진행합니다. (박스 수령 2주 후 리뷰 요청 메일 → Shelf에서 리뷰 작성 → 크레딧 지급 → 다음 박스 큐레이션에서 사용)
2. **추천 시스템 실험** — 협업 필터링(비슷한 사용자의 선택)과 콘텐츠 기반 필터링(피부 타입 적합성)을 결합해 제품 발견(discovery)을 유도하고, 트렌딩 제품을 블렌딩하여 노출합니다. 추천 유형별 태그/라벨을 부착해 사용자가 차이를 이해할 수 있게 합니다.
3. **리뷰 리워드 프로그램 (E1 후속)** — E1 결과를 전제로 한 전면 보상 체계의 1차 구현입니다. 리뷰/피드백 작성에 포인트(화폐성)와 배지/레벨(비금전 인정)을 이원 트랙으로 지급하고, A/B 실험이 아닌 단계적 론칭(Phase 1 MVP → 2 → 3)으로 진행합니다. Ipsy·Birchbox·Sephora·Google Local Guides·Yelp Elite 등 미국 시장 레퍼런스 구조를 벤치마크했습니다.

## 문서 규칙

- 주간 플래닝 파일명: `docs/planning/YYYY-Wnn-product-planning.md` (ISO 주차 기준, 매주 초안 작성 → 플래닝 미팅에서 확정)
- PRD 파일명: `NN-slug.md` (NN은 우선순위 순번)
- 실험 상태: `Draft` → `Review` → `Approved` → `Running` → `Analyzing` → `Done`
- 프로그램(비실험, 단계적 론칭) 상태: `Draft` → `Review` → `Approved` → `Phase 1` → `Phase 2` → `Phase 3` → `GA`
- 모든 실험은 시작 전 [00-experiment-overview.md](docs/experiments/00-experiment-overview.md)의 공통 가드레일 지표를 확인합니다.
