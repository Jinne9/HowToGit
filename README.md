# 작성자
201340130 이호진

# 과제 
마크다운 언어로 GitHub 협업 방법을 소개합니다!

# GitHub 사용 & 협업 방법
1. 설치 사이트에 들어가 Gut 을 설치합니다. ( https://gitforwindows.org/ )
2. 계정을 생성합니다.
		<br>- cmd 창에서 git version 으로 설치 확인을 한 후에,
		<br>- git config --global user.name "사용할이름" 
		<br>- git config --global user.email 사용할이메일 으로 본인의 사용계정을 설정해줍니다.
3. Git 계정에서 새로운 Project 를 생성해 줍니다.
		<br>- 본인의 Git 저장소 주소가 생성됩니다.
3. 본인의 드라이브에 Git을 연동할 폴더를 만들어줍니다.
# Git 에 파일 추가/편집 -- Commit
4. cmd 창에서 'cd' 명령어를 통해 연동폴더를 찾아간 후에 본인의 Git 저장소 주소를 입력해 연동해줍니다.
		<br>- git clone 저장소주소
5. 'cd' 명령어를 통해 연동된 저장소 폴더를 찾아가 git status 를 통해 생성/수정 된 파일 정보를 확인합니다.
		<br>- git status
		<br>- 빨간색으로 나오는 경우 변경된 사항이 적용이 되지 않은 상태 이므로 가이드라인을 따라 적용해줍니다.
6. 변경된 사항을 'Commit' 하는 작업을 진행합니다.
		<br>- Commit :  내가 수정한 코드를 나의 로컬 저장소인 컴퓨터에 반영하는 것을 뜻함.
		<br>- git add * or git add 파일이름
7. git add 를 하면 적용이 되고 코드 네임이 빨간색 > 초록색 으로 변합니다.
8. 그 후 git commit 을 통해 수정사항에 대한 코멘트를 달아줍니다.
		<br>- git commit -m "plese wrtie english here about Changes"
9. 마지막으로 git push 를 통해 Git 허브인 Repository 의 작업 결과물을 push 해줍니다.
		<br>- git push
		<br>- git stats > git add 'something' > git commit > git push 의 루트로 파일을 생성/수정/공유 해줍니다.
# Git 의 브렌치를 통한 협업 Play -- Branch
10. 저장소 폴더에서 git branch 를 통해 자신의 branch 를 확인합니다.
		<br>- Branch : 협업이 가능하도록 하는 가지. Master 브렌치를 두고 본인의 브렌치에서 작업한 결과물을 최종적으로 Master 브렌치에 Merge 시키는 식으로 협업이 진행된다.
		<br>- git branch
11. 새로운 브렌치를 만들어준다.
		<br>- git branch newbranch
12. 기본 master 브렌치에서 새로 만들어준 newbranch 로 사용 브렌치를 이동한다
		<br>- git checkout newbranch
13. 이 브런치에서 새로 파일을 생성/수정 하고 >> git push 작업하까지 하고 새로운 브렌치에 작업결과물을 넣는다.
		<br>- git push --set-upstream origin newbranch
14. GitHub 웹에 새로운 브렌치가 생기고 본인의 결과물이 나타난다.
15. 다시 새로운 브렌치에서 마스터 브렌치로 이동할 경우, 저장소 폴더에 파일이 newbranch > master branch 작업결과물로 바뀌어 있다.
16. 본인의 브렌치에서 작업이 끝난 경우, master branch 와 newbranch 의 결과물을 merge 시켜준다.
		<br>- 통합하고 싶은 브렌치로 이동한다.
		<br>- git checkout master
		<br>- 반영시킬 브랜치를 머지시킨다.
		<br>- git merge newbranch
		<br>- master <<< newbranch 를 통합시킨다.
17. Merge 가 끝난 후 git push 를 통해 Github 저장소에 반영시킨다.
		<br>- git push
18. 끝!


