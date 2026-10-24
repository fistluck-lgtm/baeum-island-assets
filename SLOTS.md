# 슬롯 목록

## 현재 채운 슬롯 (2026-10-21)

✅ 채움 (39개 파일): `tree_fruit`(2종) · `tree_pine`(5종) · `tree_palm` · `rock`(2종) · `bush` · `flower`(4종) · `house`(같은 집 6가지 색: 노랑·하늘·분홍·민트·빨강·보라 → 모둠원 집마다 다른 색) · `board` · `bridge` · `fountain` · `lighthouse` · `npc_otter`(달수) · `npc_penguin`(펭이, 손 흔들기 동작) · 가구 10종 + 선물 가구 `furn_dino`·`furn_balloon`

⬜ 아직 기본 모델: `player_*` 동물 주민 6종 · `npc_sheep` · `shop` · `stage`

- `npc_sheep`: *Sheep animation lowpoly*는 사실적인 회색 양이라 섬의 귀여운 분위기와 맞지 않아 기본 몽실이를 그대로 썼어요. 하얗고 동글동글한 *cute sheep chibi*를 추천해요.

- `shop`: 올려 주신 *Low poly generic shop*은 **Sketchfab Standard 라이선스**라 공개 저장소에 올릴 수 없어요. CC0/CC BY 상점 모델을 찾아 주세요.
- `stage`: *Wooden Stage with Bleacher style Seating Benches*는 Sketchfab Standard 라이선스라 쓸 수 없어요. CC0/CC BY의 *wooden stage*, *festival stage*를 찾아 주세요.
- `shop`: *Shop (MRX)*은 회색 콘크리트 건물이라 기본 상점을 그대로 썼어요. 파스텔 톤 *market stall*, *cute shop*을 추천해요.
- 같은 슬롯에 여러 모델을 넣으려면 manifest에서 `"variants": [ {...}, {...} ]` 로 적으면 섬 곳곳에 섞여서 나와요.
- 모델 안의 열매를 흔들기 표시로 쓰려면 `"fruitNodes": "^Fruits"`처럼 열매 부분 이름을 적어요.

`models/슬롯이름.glb` 로 올리고 `manifest.json`에 같은 슬롯 이름으로 적으면 됩니다.
추천 검색어는 스케치팹에서 영어로 검색할 때 쓰세요. (`low poly` 를 붙이면 가볍고 귀여운 모델이 잘 나와요)

**우선순위**: ⭐ 화면에 많이 나와서 바꾸면 분위기가 확 달라지는 것부터 하세요.

| 우선 | 슬롯 | 게임 속 역할 | 자동 크기 | 추천 검색어 |
|---|---|---|---|---|
| ⭐ | `tree_fruit` | 열매 나무 (흔들기) | 높이 4.6m | low poly apple tree, cute fruit tree |
| ⭐ | `tree_pine` | 소나무 | 높이 5.2m | low poly pine tree |
| ⭐ | `tree_palm` | 해변 야자수 | 높이 6m | low poly palm tree |
| ⭐ | `house` | 학생 집 (모둠원마다 1채) | 높이 4.2m | cute low poly house, cottage |
| ⭐ | `player_cat` | 고양이 주민 | 높이 1.7m | cute cat character animated |
| ⭐ | `player_dog` | 강아지 주민 | 1.7m | cute dog character |
| ⭐ | `player_rabbit` | 토끼 주민 | 1.9m | cute bunny character |
| ⭐ | `player_bear` | 곰 주민 | 1.7m | cute bear character |
| ⭐ | `player_fox` | 여우 주민 | 1.7m | cute fox character |
| ⭐ | `player_panda` | 판다 주민 | 1.7m | cute panda character |
|  | `npc_sheep` | 몽실이 (부탁 문제) | 1.8m | cute sheep low poly |
|  | `npc_otter` | 달수 (상점) | 1.9m | cute otter / beaver character |
|  | `npc_penguin` | 펭이 (복습 노트) | 2.0m | cute penguin low poly |
|  | `rock` | 돌 (두드리기) | 1.1m | low poly rock |
|  | `bush` | 덤불 | 1.0m | low poly bush |
|  | `flower` | 꽃 (꽃 따기) — 많이 나오니 아주 가벼운 것만 | 0.5m | low poly flower |
|  | `shop` | 달수 상점 건물 | 5.5m | low poly shop, market stall |
|  | `board` | 모둠 공사 게시판 | 2.6m | notice board, wooden sign board |
|  | `bridge` | 1단계: 다리 | 길이 7.4m | wooden bridge low poly |
|  | `fountain` | 3단계: 분수대 | 2.8m | fountain low poly |
|  | `stage` | 4단계: 축제 무대 | 폭 6.2m | wooden stage, festival stage |
|  | `lighthouse` | 5단계: 등대 | 10m | lighthouse low poly |
|  | `furn_pot` | 가구: 꽃 화분 | 1m | flower pot |
|  | `furn_mailbox` | 가구: 우체통 | 1.4m | mailbox |
|  | `furn_bench` | 가구: 벤치 | 폭 1.8m | park bench low poly |
|  | `furn_mat` | 가구: 피크닉 매트 | 폭 2m | picnic blanket basket |
|  | `furn_lamp` | 가구: 가로등 | 2.9m | street lamp low poly |
|  | `furn_parasol` | 가구: 파라솔 | 2.6m | beach umbrella |
|  | `furn_campfire` | 가구: 모닥불 | 0.8m | campfire low poly |
|  | `furn_arch` | 가구: 꽃 아치 | 2.8m | flower arch |
|  | `furn_swing` | 가구: 그네 | 2.5m | swing set |
|  | `furn_windmill` | 가구: 작은 풍차 | 4m | small windmill low poly |

## 모델을 고를 때

- **같은 작가의 팩(pack)** 에서 여러 개를 고르면 색감이 맞아서 훨씬 자연스러워요. (예: *low poly nature pack*)
- 너무 사실적인 모델보다 둥글고 파스텔 톤인 모델이 배움섬 분위기에 맞아요.
- 땅·바다·강은 게임이 직접 그려서 따로 모델이 필요 없어요.
- 특정 게임·만화 캐릭터(예: 닌텐도 캐릭터)를 그대로 따라 만든 팬아트 모델은 저작권 문제가 있을 수 있으니 피해 주세요.

## 새로 생긴 슬롯 (공사 6~8단계 · 선물 가구)

| 슬롯 | 쓰이는 곳 | 추천 검색어 |
|---|---|---|
| `playground` | 6단계 놀이터 | `playground low poly`, `kids playground stylized` |
| `greenhouse` | 7단계 온실 | `greenhouse low poly`, `glass greenhouse stylized` |
| `observatory` | 8단계 천문대 | `observatory low poly`, `telescope tower stylized` |
| `furn_fishstatue` | 물고기 도감 완성 선물 | `fish statue gold low poly`, `fish trophy` |
| `furn_bugframe` | 곤충 도감 완성 선물 | `insect frame`, `butterfly display case` |
| `furn_dino` | 화석 도감 완성 선물 | `dinosaur skeleton low poly`, `fossil skeleton cartoon` |
| `furn_balloon` | 학급 축제 선물 | `balloons low poly`, `balloon bunch` |

모델이 없으면 게임 안 기본 모델로 보여요.
