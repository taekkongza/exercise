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






