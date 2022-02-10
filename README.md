# Git Make Commnd

01. `echo "# test" >> README.md` : echo 내용 작성, >> (파일 만들기 & 내용 넣기)
02. `git init` : .git 폴더 만들기 ( github 브라우저 연동하기 위함 )
03. `git add README.md` : add 는 commit 전 단계
04. `git commit -m "make md file"` : commit 은 push 전 단계
05. `git status` : 현재 로컬 저장소 경로에서의 git 상태
06. `git branch -M main` : branch 를 main 으로 바꾸는 과정, 처음 한 번만 하고 안해도 됨.
07. `gh repo create "repo NAME"` : github 브라우저에서  개인 계정 원격 저장소에 레포지토리 생성.
08. `git remote add origin https://github.com/iehosa/"repo NAME".git`: 원격 저장소로 연결.
09. `git remote -v` : 원격 저장소 목록
10. `git push -u origin main` : push는 로컬 저장소의 변동사항을 원격 저장소로 업로드.
11. `git pull origin master` : pull은 원격 저장소의 변경사항은 로컬 저장소로 임포트.

# Git Modify Commnd

01. `git reset HEAD "파일명"` : add 취소, 파일명 없어도 됨.
02. `git reset --soft HEAD^` : add 상태로 commit 취소.
03. `git reset HEAD^` : add, commit 둘다 취소.
04. `git reset HEAD~2` : 마지막 2개의 commit 취소.
05. `git reset --hard HEAD^` : add, commit 둘다 취소하고 로컬 저장소에서 삭제.
06. `git commit --amend` : commit 메시지 변경.
