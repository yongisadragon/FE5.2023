# 🛠️ Git & GitHub

Git-GitHub은 솔직히 나에겐 버거웠다.. 처음 배우기도 하지만 이해하기 위해 더 공부했다. 어디까지나 복습차원에서 기록하는 것이고, 설명하는 것이 어색할 수도 있다. 이 부분은 나중에 여러번 수정을 거칠 예정이다..

>_솔직히 이해가 안 되는데요..?_

우선 Git과 GitHub는 다르다. 이름에서도 알 수 있듯, Git은 로컬이 연결된 분산 버전 관리 '시스템'이고, GitHub은 루비 온 레일즈를 기반으로 만들어진 '웹서비스'이다. Git은 내컴퓨터(로컬)에 설치되는 `Software`이고, GitHub은 웹상에서 구동되는 `Service`이다. Git은 처음에 파일을 설치하고 초기설정을 해준다.

시작에 앞서.. 깃허브 초기 Repository의 설정을 하며 겪은 스트레스를 먼저 소개하겠다.

이것은 GitHub에서 Repository를 생성하고, 내 로컬로 불러오는 것(Clone)에 대한 설명이다. 먼저, 첫 번째로 헷갈렸던 것은 당장 초기 레파지토리를 생성할 때부터이다. 왜 README를 생성하고 안 하고 안내되는 문구가 다를까?.. 초보인 나에겐 힘든 일이었다..

조금 알아본 결과, README를 만든 채로 시작하면 깃허브에 바로 레파지토리가 생성되지만, 체크를 해제한 채로 생성하면 다들 알고 있는 그 페이지 `.. or create a new repository on the command lin` 혹은 `… or push an existing repository from the command line`이다. 위아래 차이도 모르겠고, 이걸 `어디에` `어떻게` `왜` 붙이는지도 이해가 안 됐다. 쉽게 설명하면 저 두 종류의 텍스트 박스 내용에는 `로컬과 깃헙을 이어주기 위한 내용`들이 들어있다고 보면 된다. 무턱대고 로컬 컴퓨터가 깃허브(원격 저장소) 연결될 수는 없지 않은가.. 

```
-init(저장소 만들기)
-add(상태추적)
-commit(상태기록)
-branch(일종의 공동채널..?)
-remote~(원격 저장소의 주소 연결)
-push(보내기) 
```

현재 이해하고 바로는 이런 의미인 듯 하다.. 정확한 용어 설명이 아니라도 이해바란다. 어찌됐든 로컬의 특정 파일위치에서 터미널(CLI든 코드에디터든)에 복붙하면 `원격 저장소와 로컬이 연결되는 주문`인 것이다.
___

# 🔁 원격 저장소와 로컬


오늘 배운 내용에 따르면, GitHub을 사용하여 깃헙과 로컬을 오가며 협업하기 위해 굵직하게 다음 단계만 기억하면 된다고한다. (아래 내용들은 원격 저장소의 링크를 git clone을 통해 원격 데이터들의 코드들 컴퓨터에 받아온 이후이다.)

```
$ mkdir filename
$ cd filename
$ git clone https://github.com/id/clone-filename.git .
```

[멋사FE5기 동료분의 URL강의](https://velog.io/@codenest/%EA%B6%81%EA%B8%88%ED%95%B4%EC%84%9C-%EC%B0%BE%EC%95%84%EB%B3%B8-URL%EC%9D%84-%EC%9E%85%EB%A0%A5%ED%95%98%EC%84%B8%EC%9A%94-2)
- [ ]

  * __git pull__
  * __git add .__
  * __git commit -m ' '__
  * __git push__

`git pull`은 말그대로 깃헙에서 내 컴퓨터 내용을 끌어오는 것이다.

`git add`는 pull로 받아온 데이터들 수정하고 다시 더하는 것이다. 공백+ . 은 전부 더한다는 뜻. 특정파일명을 입력해서 더할수도 있다.

`git commit`은 add한 파일과 데이터들을 저장소에 올리는 것이다. `-m '리얼 마지막'`은 일종의 버전 기록. 1차,, 2차,, final.. 이런 느낌이라고 보면 된다.

`git push`가 이루어지면 이제 GitHub의 Repository(원격 저장소)로 데이터를 쏘는 것이다.

add와 commit에 대해 좀 더 덧붙이자면, 작업한 폴더 안의 파일들을 기록에 남기고 싶다면 미리 골라 git add한다고 한다. 그것을 staging area로 보낸다고 하고(그래서 git add하는 것을 스테이징한다고도 한다.) 그 이후 git commit하는 것은 데이터를 repository(기록 저장소)에 옮기는 것이다.

여기까지가 현재까지 흡수한 내용들이다. 실제로 협업을 하면서 더 자연스러워지겠지만.. 아무튼 개발과 관련된 공부들은 복잡하긴 하지만 익숙해지는 것 밖엔 길이 없다.. 나.. 할 수 있겠지?
