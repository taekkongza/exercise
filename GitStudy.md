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
작업 폴더 : 파일들 -> 저장할 파일 git add --> staging area --> git commit --> repository
