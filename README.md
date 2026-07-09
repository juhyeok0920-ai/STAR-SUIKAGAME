# ✨ Star Suika Game (스타 머지: 원소의 기원)

> **Matter.js 물리 엔진을 탑재한 우주 테마의 2D 행성 합성 샌드박스 게임입니다.**  
> 수소(H)부터 시작하여 철(Fe) 중심핵을 완성하고 초신성 폭발(Supernova)을 유도하세요!

<br>

## 🌌 게임 소개 (Game Overview)
이 게임은 기존의 유명한 '수박 게임(Suika Game)' 룰을 우주 물리학 테마로 재해석한 브라우저 게임입니다. 
단 하나의 HTML 파일로 구동되며, 강력한 2D 리지드 바디 물리 엔진인 **Matter.js**를 사용하여 부드러운 회전, 백스핀, 그리고 구석에 짓눌려도 파고들지 않는 정교한 충돌 판정을 제공합니다.

* **플레이 방법**: 마우스를 움직여 원소를 조준하고, 클릭하여 떨어뜨립니다.
* **승리 조건**: 규소 연소 단계를 거쳐 최종 원소인 **철(Fe)**을 합성하면 초신성 폭발과 함께 게임에서 승리합니다.
* **패배 조건**: 원소들이 통제 한계선(데드라인)을 넘은 상태로 2초 이상 버티지 못하면 중력 균형이 무너져 블랙홀로 붕괴(게임 오버)합니다.

<br>

## 🛠️ 기술 스택 (Tech Stack)
* **Language:** HTML5, CSS3, JavaScript (Vanilla JS)
* **Physics Engine:** [Matter.js](https://brm.io/matter-js/) (v0.19.0)
* **Hosting:** GitHub Pages

<br>

## 🌟 주요 특징 (Key Features)
* **Matter.js 기반의 정밀한 물리 연산:** 자체 튜닝된 반발계수(Restitution)와 마찰력(Friction)을 통해 리얼한 항성 간의 마찰과 구르기를 구현했습니다.
* **샌드위치 끼임/관통 방지:** 프레임당 다중 연산 처리 서브루틴을 활용하여 거대 행성이 작은 행성을 구석에서 짓눌러도 벽면 밑으로 파고드는 물리 버그를 완벽히 차단했습니다.
* **가변 질량 시스템:** 원소의 단계(Level)가 높아질수록 크기뿐만 아니라 밀도(Density)와 무게(Mass)가 동적으로 증가하여 아래쪽 원소를 묵직하게 압박하는 사실적인 손맛을 줍니다.
* **화려한 엔딩 시퀀스:** 철(Fe) 합성 성공 시 주변 원소들을 모두 흡수하며 화면이 진동하는 초신성 폭발 애니메이션 연출이 포함되어 있습니다.

<br>

## 🧪 항성 진화 단계 (Stellar Evolution Tree)
원소는 합성될 때마다 다음 단계로 진화합니다:

| 레벨 | 원소 기호 | 원소 이름 | 스폰 여부 |
| :---: | :---: | :---: | :---: |
| Lvl 0 | **H** | 수소 (Hydrogen) | 스폰 가능 (60%) |
| Lvl 1 | **He** | 헬륨 (Helium) | 스폰 가능 (30%) |
| Lvl 2 | **C** | 탄소 (Carbon) | 스폰 가능 (10%) |
| Lvl 3 | **O** | 산소 (Oxygen) | 조합 전용 |
| Lvl 4 | **Ne** | 네온 (Neon) | 조합 전용 |
| Lvl 5 | **Mg** | 마그네슘 (Magnesium) | 조합 전용 |
| Lvl 6 | **Si** | 규소 (Silicon) | 조합 전용 |
| Lvl 7 | **Fe** | 철 (Iron) | **최종 진화 (승리)** |

<br>

## 🚀 실행 방법 (How to Run)
별도의 빌드나 서버 설치 과정이 필요하지 않습니다.

1. 이 저장소를 클론하거나 코드를 다운로드합니다.
   ```bash
   git clone [https://github.com/YOUR_USERNAME/star-suika-game.git](https://github.com/YOUR_USERNAME/star-suika-game.git)
