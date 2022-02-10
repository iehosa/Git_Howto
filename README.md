# Git Start

## Git Make Commnd

01. `echo "# test" >> README.md` : echo 내용 작성, >> (파일 만들기 & 내용 넣기)
02. `git init` : .git 폴더 만들기 ( github 브라우저 연동하기 위함 )
03. `git add README.md` : add 는 commit 전 단계
04. `git commit -m "커밋내용"` : commit 은 push 전 단계
05. `git status` : 현재 로컬 저장소 경로에서의 git 상태
06. `git branch -M main` : branch 를 main 으로 바꾸는 과정, 처음 한 번만 하고 안해도 됨.
07. `gh repo create "레포지토리 이름"` : github 브라우저에서  개인 계정 원격 저장소에 레포지토리 생성.
08. `git remote add origin https://github.com/iehosa/"repo NAME".git`: 원격 저장소로 연결.
09. `git remote -v` : 원격 저장소 목록
10. `git push -u origin main` : push는 로컬 저장소의 변동사항을 원격 저장소로 업로드.
11. `git pull origin main` : pull은 원격 저장소의 변경사항은 로컬 저장소로 임포트.

## Git Modify Commnd

* `git reset HEAD "파일명"` : add 취소, 파일명 없어도 됨.
* `git reset --soft HEAD^` : add 상태로 commit 취소.
* `git reset --mixed HEAD^` : add, commit 둘다 취소.
* `git reset HEAD~2` : 마지막 2개의 commit 취소.
* `git reset --hard HEAD^` : add, commit 둘다 취소하고 로컬 저장소에서 삭제.
* `git commit --amend` : commit 메시지 변경.

## Git Error 01

```
 ! [rejected] master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/devAon/SOPT-SERVER-nodejs.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details. 
```
- pull 한 다음 push 진행한다.
- `git push -u origin +main` : +는 강제 푸쉬하는 것인데, 강제 푸쉬하게되면 모든 작업이 다 사라지고 커밋된 파일만 남는 상황이 발생할 수도 있기 때문에 하지 않는 것이 좋다.
