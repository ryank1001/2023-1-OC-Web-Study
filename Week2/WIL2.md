## add commit push <br>
### 1. add  

  Working directory 내에서 작업한 내용을 add 명령어를 통해서 staging area로 옮길 수 있다.

### 2. commit

  staging area에서 local repository로 옮기면서  컴퓨터에 현재 상태를 저장한다. commit을 한 시점부터 저장이 시작되며 추후 다시 돌아 올 수 있게 된다.

### 3. push

  local repository에서 remote repository로 옮기면서 git에서 이 파일을 관리하도록 한다.
<br>
<br>
<br>

## pull과 fetch의 차이점

  pull은 remote repository에서 브랜치를 가져와서 자신의 local repository와 병합을 하는데에 반해, fetch는 브랜치를 가져온 후 이를 병합하지 않고 이후 merge 명령어를 활용해 병합할 수 있다.