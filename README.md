# Intro
- 결합게임을 Dart의 UI 프레임워크 Flutter를 이용해 하이브리드앱으로 구현하는 프로젝트

# Skill
- Dart, Flutter, Node.js, MariaDB, 배포-Heroku(예정)

# 진척사항
- 2021.01.17
  - 그리드뷰 구현
- 2021.01.18
  - FlatButton에 이미지 추가
  - 랜덤문제&정답('합') 생성 로직 구현 (List, Map 사용)
- 2021.01.19
  - StatefulWidget에서 버튼 클릭시 이미지 Opacity를 변경하는 Animation 적용
  - button의 onPressed가 발동되어 build 위젯이 새로고침될 때마다 랜덤문제가 새로 생성됨 
    -> 게임생성로직을 build 위젯 외부로 이동
    -> 생성된 게임은 그대로 있되, button의 state만 변경되도록 적용
  - button에 padding 적용 (테두리선)
  - onPressed 시에 체크 상태값 설정을 함수에서 처리하도록 적용 (funcCellChecked)
    - Cell을 3개 이상 선택 시, 더 이상 선택할 수 없도록 처리

- 다음 진척예정사항: 
  - '제출' 버튼 생성
  - '제출' 버튼으로 선택된 3개의 답을 ansList와 비교
  - 정답이면 score++
