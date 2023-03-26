##Week2 
git은 파일의 변경사항을 추적하고 협업 작업을 조율해주는 것  

파일의 4가지 상태
* 추적 X (Untracked)
* 변경 X (Unmodified)
* 변경 O (Modified)
* staged  

내 컴퓨터  
working directory - staging area - local repository  


git add 명령어를 통해 Staging Area 에 변화를 쌓음  

git commit 명령어를 통해 repository로 옮기며 하나의 커밋이 됨  

* .git = 로컬 리포지토리

내 컴퓨터  
working directory - staging area - local repository  
외부저장소  
remote repository  
(깃허브가 외부저장소 역할을 함)  
-> 공통의 외부 저장소가 있어야 서로 자료 공유 가능  

----
git init  ; git 시작  
local repository = .git directory (폴더)  
.git 폴더가 내 repository 가 된 것  

git add . 는 폴더에 있는 내용이 다 들어감  
git add 는 변경내용을 스테이지로 올리는 것  
git status 현 상태 보여줌  
git commit -m "first commit"  
>>-m 은 메시지의 약자  

git branch -m main (master 를 main 으로 바꿈)  
git remote add origin https://github.com/binary-ho/doitexactly.git 는 
컴퓨터 로컬 터미널에 쳐줌  

그럼 내가 사용할 리포지토리와 깃허브가 연결된 것  

git push -u origin main 
push 를 이용해서 로컬 리포지토리의 내용을 리모트 리포지토리로 올릴 수 있음  
----
git add 는 변경내용을 스테이지로 올리는 것  

git commit은 스테이지에 올라온 파일을 커밋하는 것  
(커밋 ; 깃에서 버전을 만드는 것)  

git push : 현재 branch에서 새로 생성한 commit들을 원격 저장소에 업로드  

git fetch 는 가져온 원격저장소 내용을 로컬에 영향 x   
git pull 은 가져온 원격저장소 내용을 로컬에 병합   
