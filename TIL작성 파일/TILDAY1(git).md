[TIL]Day 1 (git)

주로 혼자 개발을 하여 branch를 혼자 사용하여 몰랐던 기능들

amend : 기존의 commit 내용을 수정하는 방법 / branch를 혼자 사용 할 때만 사용!

    사용법 - git add 파일명,  git commit --amend 명령어 순서로 수행시 commit의 내용을 변경할 수 있다.
 

stash : branch를 옮겨야 할 때 새로운 commit을 생성하지 않고 임시 저장 후 branch를 옮기는 방법

    사용법 - git stash -m '메세지 내용' 후에 branch를 이동하여 작업한다. 다시 branch로 돌아와 git stash apply 명령어로 작업을 불러온다.  git stash list 명령어로 저장된 목록을 확인할 수 있다.
 

reset - 커밋을 되돌릴 때 사용한다 / 개인 branch에서만 사용하는 것을 권장

    사용법 - git reset -mixed 커밋 아이디, git hard 커밋아이디 or ~숫자 //  mixed는 변경 내용은 남기고 commit 이력을 되돌린다.  hard는 변경 내용을 모두 지우고 원하는 아이디 또는 현재부터 숫자만큼 이전 이력으로 돌아간다.
 

cherry-pick - 다른 브랜치의 원하는 commit만 골라서 merge한다 / 파일을 되돌려서 merge할 필요가 없다!

    사용법 - git cherry-pick 커밋 아이디(다른 브랜치의 커밋)