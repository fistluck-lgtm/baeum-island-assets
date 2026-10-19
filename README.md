# 배움섬 3D 에셋 저장소

배움섬 게임이 이 저장소의 `manifest.json`을 읽어서, 적혀 있는 슬롯만 스케치팹 모델(GLB)로 바꿔 끼웁니다.
**적혀 있지 않은 슬롯은 게임에 들어 있는 기본 모델이 그대로 나오니까**, 마음에 드는 모델을 하나씩 천천히 추가하면 됩니다.

## 1. 저장소 만들기 (처음 한 번)

1. GitHub에서 **새 저장소 `baeum-island-assets`** 를 **Public**으로 만듭니다. (Private이면 학생 기기가 받을 수 없어요)
2. 이 폴더의 파일(`manifest.json`, `models/`, `README.md`, `SLOTS.md`)을 그대로 올립니다.
3. 다른 이름으로 만들었다면 선생님 화면 → ⚙️ 설정 → `에셋저장소`에 `계정/저장소이름`을 적어 주세요.

## 2. 스케치팹에서 모델 고르기

- 검색 후 왼쪽 필터에서 **Downloadable** 을 켜고, 라이선스는 **CC0** 또는 **CC BY**만 고르세요.
  (CC BY-NC는 학교 수업 사용은 대체로 괜찮지만 애매하면 피하는 게 안전해요. *NoDerivatives(ND)* 와 *Editorial* 은 쓰지 마세요.)
- 다운로드할 때 **glTF Binary (.glb)** 를 고릅니다.
- **파일 크기 2MB 이하**를 권장해요. 30대의 태블릿이 같은 와이파이로 동시에 받기 때문이에요.
  모델 페이지의 *Triangles* 가 **1만 개 이하**인 로우폴리(Low Poly) 모델이 가볍고 이 게임 분위기와도 잘 맞아요.
- 큰 파일은 https://gltf.report 에 올려서 *Export → Compress(Draco 제외)* 로 줄일 수 있어요.

## 3. 슬롯에 넣기

1. 받은 `.glb` 파일 이름을 슬롯 이름으로 바꿔 `models/` 폴더에 올립니다. 예) `models/tree_fruit.glb`
2. `manifest.json`에 한 줄 추가합니다. (`manifest.example.json` 참고)

```json
{
  "version": 1,
  "models": {
    "tree_fruit": { "file": "models/tree_fruit.glb", "credit": "\"Apple Tree\" by 작가 (CC BY 4.0) https://sketchfab.com/3d-models/..." }
  }
}
```

| 항목 | 뜻 |
|---|---|
| `file` | 저장소 안의 파일 경로 (필수) |
| `credit` | 저작자 표시. **CC BY 모델은 꼭 적어 주세요.** 게임 안 📋 메뉴의 ‘3D 모델 저작자 표시’에 나와요 |
| `scale` | 자동 크기 조절 뒤 추가 배율 (기본 1) |
| `rotY` | 모델이 뒤를 보고 있으면 `180`처럼 돌리기(도) |
| `y` | 땅에 묻히거나 뜨면 위아래 조정 |
| `height` | 자동으로 맞출 높이(m)를 직접 정하기 |

크기는 게임이 슬롯마다 알맞은 높이로 **자동으로 맞춰요**. 그래서 대부분은 `file`과 `credit`만 적으면 돼요.

## 4. 반영 확인

- 게임은 jsDelivr CDN으로 받아요. 올린 뒤 바로 안 바뀌면 아래 주소를 브라우저에서 한 번 열어 캐시를 지우세요.
  `https://purge.jsdelivr.net/gh/계정/baeum-island-assets@main/manifest.json`
  (모델 파일을 바꿨다면 그 파일 주소도 같은 방식으로)
- 학생 화면을 새로고침하면 적용됩니다. 불러오기에 실패한 모델은 기본 모델로 자동으로 돌아가요.

## 캐릭터 모델 팁

- `player_*`, `npc_*` 슬롯은 애니메이션이 들어 있으면 이름에 `idle` / `walk`(또는 `run`)가 들어간 클립을 자동으로 써요.
- 애니메이션이 없는 모델도 괜찮아요(그냥 미끄러지듯 움직여요). 기본 모델은 걷는 동작이 들어 있어요.
- 학생 캐릭터는 같은 동물을 고른 친구끼리 같은 모델을 써요. 옷 색깔은 기본 모델에서만 보여요.

슬롯 전체 목록과 추천 검색어는 [SLOTS.md](SLOTS.md)에 있어요.
