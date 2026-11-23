# 02 구조 설계 · 시공 계획: 스파게티 교량

지점 간 108cm 스파게티 트러스 교량입니다. 과제 조건은 중앙 3kg 재하, 모든 부재 2가닥입니다.

AI와 만든 처음 3D 설계에서 멈추지 않았습니다. Claude와 함께 설계를 다시 검토해 3힌지 A형으로 고친 뒤, 실제로 만드는 순서를 18단계 3D 시뮬레이션으로 짰습니다.

| 파일 | 내용 | 바로 열기 |
|---|---|---|
| `first-3d-design.html` | 처음 3D 설계. 부재 335개, 부재 힘을 압축(빨강)·인장(파랑)으로 표시 | [열기](https://kwontaegeun.vercel.app/02-structural-design/first-3d-design.html) |
| `construction-sequence-simulation.html` | 개선 설계의 시공 순서. 받침대·지그 제작, 접착 시험, 부재 생산, 다리 조립, 세우기, 3kg 재하까지 18단계 | [열기](https://kwontaegeun.vercel.app/02-structural-design/construction-sequence-simulation.html) |
| `images/` | 포트폴리오에 쓴 그림. 3D 설계 1장, 시공 장면 4장(11·13·14·18단계) | |

## 계산 결과 (시뮬레이션에 적힌 값)

| 항목 | 값 |
|---|---|
| 최소 부재 여유 (선형 해석, 자중 포함) | 처음 설계 약 1.85배 → 개선 설계 약 3.5배 |
| 이음·제작 오차를 넣은 첫 파괴 하중 (보통 품질 가정) | 약 4.6kg |
| 3kg에서 최대 처짐 (인장재는 실) | 약 3.3mm |

모두 계산값입니다. 접합부 강도와 제작 오차는 가정을 세워 넣었습니다.
