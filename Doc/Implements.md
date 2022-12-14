## 구현해야 할 것들

- 과거 주식 데이터의 취득
  - 게임 입장 시에 랜덤한 종목의 랜덤한 일정 구간을 취득, 이름 등 간략한 정보를 출력
  - 게임성을 위해서, 주가의 극적 변화나 꾸준한 변동성을 보이는 구간을 찾아내는 알고리즘 필요
- 게임성을 위한 기능
  - 클라이언트 내에서 게임 조작 시 최대한 지연 없이 빠른 피드백 반영
  - AI / 멀티 매칭 선택
  - 게임 내에서 주식 지식 기반이 적은 플레이어를 위한 튜토리얼 기능
  - 플레이어 정보 (닉네임, 점수, 프로필 사진 등)
  - 일정한 조건을 달성하면 해금되는 업적 기능
  - 종목 검색 기능이 있어, 그 종목의 정보와 과거 데이터를 그래프로 출력해주는 기능
- In-Game 기능
  - 캔들 그래프 / 꺾은선 그래프
    - 버튼 등 조작으로 두 그래프의 Swap 출력 기능
    - 게임 시간에 따른 그래프의 실시간 갱신
  - 버튼 조작 시에 플레이어의 당시 수익률 퍼센테이지포인트 계산 후 최신화된 수치 출력
    - 상승/하락 예측을 통한 수익 계산 알고리즘 필요
- 멀티플레이어 기능
  - 랜덤 매칭을 통한 경쟁 구현
  - 게임 중 사용 가능한 아이템 구현
  - 랭킹 시스템을 위한 점수 기능, 이를 저장/계산하기 위한 서버 구현
  - 친구 기능과 친선전 기능, 이 데이터를 저장하기 위한 서버
- Auto-Trading
  - 다양한 Auto-Trading 전략 수집, 이를 알기 쉽도록 간단하게 개량 필요
  - 항목을 단순화한 여러 지표 및 팩터를 구현, 여러 가짓수를 조합해 본인만의 전략 구축
- AI 기능
  - Auto-Trading의 선구현이 필요
  - 다양한 Auto-Trading 전략을 이용한 AI로 플레이어와 경쟁
  - 전략에 따른 AI 난이도의 분화, 플레이어에게 정보 제공
  - AI가 사용한 전략을 본인의 투자에 사용 가능하도록 Copy/Paste 할 수 있는 기능

</br>

- 게임 조작 방법에 대해
  - 가능한 한 간단한 방향으로 가면 좋을 것 같음
    - 대부분의 기능은 마우스 클릭으로 해결 가능하게 함
    - 조작의 편의성을 위해, 상승/하락 예측, 그래프 Swap, 아이템 등의 주요 기능은 마우스뿐 아니라 단축키를 설정하여 이를 이용할 수 있게 함
    - 검색 기능은 주식 종목들을 카테고리화하여 출력해주고, 그 리스트에서 선택하거나 직접 타이핑을 통해 원하는 종목을 찾을 수 있게 함
    