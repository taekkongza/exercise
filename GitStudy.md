설치  
windows  
git windows -> downloads : use VS code check, override the default branch... check  
mac  
homebrew 검색 설치 --> launch pad - 터미널 - brew install git  
기본 브랜치 이믈 main으로 바꾸기  
기본에디터 VScode로 바꾸기  
  
시작  
폴더 만들기 --> 터미널  
git config --global user@email   
git config --global username  
끝  
  
VScode  
작업 폴더 만들기 --> 폴더 열기 --> 터미널 열기
git init  
작업폴더 감시
파일 생성, 코드 작성
터미널에서  
git add app.txt  
git commit -m '메세지 첫파일'
코드 추가 작성  
git add app.txt  
git commit -m "수정했음'  

모든 파일의 버전을 기록할 필요가 없어서 명령어가 2개로 나뉨  
예 : 그림파일  
1 . git add로 기록할 파일을 고른다.  
2. 고른 파일을 기록명령 git commit  
### 작업 폴더 : 파일들 -> 저장할 파일 git add --> staging area (스테이징함) --> git commit --> repository (저장소)  

여러 파일을 스테이징 git add . 

git status 상태창  
어떤 파일이 스테이징 되었는지 수정이 되었는지  

commit 내역 조회  
git log --all --oneline  

VScode   
좌측 표 - + 는 add √ 는 commit  

파일 수정후 차이 확인  
git diff  
최근 commit 와 현재 파일의 차이점 보여줌  
git difftool  파일 비교 vim 사용하여  

git difftool 커밋아이디 - 현재파일과 특정커밋 비교가능  
--> VS code에서 에디트 가능함..  
extension 에서 git graph 설치  
git log 와 똑같은 화면이 나온다.  
좌측 상단에 그래프모양 클릭 하면 변동 나온다.  


### 코드를 짜다가 에러가 나면 안되므로 파일 복사본 만들어서 거기에  먼저 코드를 짜면 안심~~
branch 기능을 이용하면 안심, commit복사본 만들기 쉬움  
터미널을 열고 git branch 작명    
git branch coupon 최근 커밋의 사본  
git switch coupon 브랜치로 이동  

git branch coupon    
git status   
git switch coupon  

main branch VS 이름 branch  

브랜치 명령어  
git branch 현재 작업중인 브랜치 목록  

git branch 이름 : 새로운 브랜치 생성  
git checkout -b 이름 : 새로운 브랜치 생성  

git checkout 이름 : 이름 브랜치로 이동  
git switch 이름 : 이름 브랜치로 이동  

git merge 이름 : 이름 브랜치를 병합  
git branch -d 이름 : 이름 브랜치 지우기  

git status : git 상태 표시
git log 최근 커밋 로그를 확인
git log --all --oneline --graph
  
branch파일을 만들고 코드 입력  -> git add .  --> git commint -m '브랜치연습'   
git switch main하면 branch파일이 안보인다.  
다시 git switch coupon하면 다시 보인다.  

coupon branch가 기능을 잘한다. -- 기능 합치기
coupon 브랜치 코드를 main 브랜치에 합치고 싶다.
1. 기준 브랜치로 이동 git switch main
2. git merge coupon
여기서 문제는 서로 다른 코드, 파일이면 괜찮으나  
동일 코드 , 동일 줄의 수정이면 수동으로 작업??  
---> conflict 에러 발생  
   1. 원하는 코드만 남기고
   2. git add .
   3. git commit -m '수정'

###

## GitFlow
1. main
2. develop
3. feature
4. release
5. hotfix
   
main : 현재 코드임 (commit) <-- 여기에 신기능 코드를 짜서 push는 절대 안돼 !!  

복사본 develop <-- 여기에 신기능 추가

feature bracn 추가해서 신기능 추가
--> 신기능이 잘돼면 합친다. merge  


  


 


 








