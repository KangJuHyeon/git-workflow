Git Workflow
=============
# README.md로 다른사람과 pull 명령어 사용해보기
### 하기 전에 원본 로컬을 fork 받아서 사람1, 사람2 이런식으로 Repo를 나눠야한다. (fork는 사람1, 사람2 둘다 받아야한다.)
### 1. 드라이버가 코드를 작성한다. add
### 2. commit -m "내용"
### 3. push origin master
### 4. 체인지
### 5. git pull 명령어를 사용하여 다른사람의 local로 가져온다.
### 6. 새로운 코드를 작성 및 commit 이후 push
### 7. 또 체인지 git pull 로 다른사람의 Repo를 자신의 local로 가져온다.
### * 주의 push는 내 Repo에 하고 pull은 상대방의 Repo를 가져온다.

# 충돌 해결
### 5번에서 다른사람이 pull로 안가져오게되면 충돌이 일어난다.
### pull을 안하고 add, commit, push를 하게 되면 에러가 나는데... 그 에러는 대부분 [rejected] master -> master (fetch first) 이런식으로 나온다.
### 이 해결법은 pull을 하게되면 해결된다.
### 예시 : git pull origin master
### 저렇게 되면 충돌이 난 부분을 수정할 수 있게 나온다. 나같은 경우는 VScode를 껐다 다시 켜야만 가능했다.
### Accept Current Change | Accept Incoming Change | Accept Both Changes | Compare Changes 이렇게 나온다.
### 1번째는 내 변경사항을 사용할 것이다.
### 2번째는 다른사람의 변경사항을 사용할 것이다.
### 3번째는 나, 다른사람의 코드를 둘다 사용할 것이다.
### 4번째는 내 코드와 비교하여 고치겠다. 라는 뜻이다.
### 설정을 다 한 후에 add, commit, push해서 사용하면 된다.

# 브랜치 만들기
### 그 전에 내가 현재 작업하고 있는 곳을 확인해야한다.
### 작업 공간을 옮긴다. ex)git checkout <브랜치 이름>
### 근데 이것을 가볍게 git checkout -b <브랜치 이름>을 사용해도 된다. -b는 branch를 생성하고 원본 브랜치로 작업공간을 이동해준다.
### 생각보다 많이 쉬운 내용이었던 것 같다. 그보다 Git Workflow 그림을 잘 이해를 해야만 쉽게 구조를 알 수 있다.
# 😅😅😅😅😅
