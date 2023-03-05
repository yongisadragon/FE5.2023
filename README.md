# 0305arrowpractic
첫 arrow는 특정 굵기를 가진 border 생성 - 각 boder에(top,right,bottom,left) 색상 부여 - 화살표를 남길 방향의 반댓방향 border소거(예를 들어 bottom을 남길거면 top제거) - 한 뒤 width,height 0으로 설정(그럼 서로 딱 붙음) - 그 다음 남길 화살표를 빼고 나머지 인접 border의 색상 transparent (***여기서 내가 한 실수***: transparent하는 방향에 색상 값을 그대로 남겨둔 상태로 뒤에 transparent붙여서 개 뻘짓함. 색상값이 들어갈 곳에 색상을 지우고 transparent 넣길바래.)
