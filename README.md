# DEMO

some description
exercise make perfect
git   
git - global information tracker  
what
is 
your name  

새로운 SSH 키를 GitHub 계정에 추가하는 방법은 다음과 같습니다:

1. **SSH 키 생성**: 먼저, 새로운 SSH 키를 생성해야 합니다. 터미널 또는 명령 프롬프트에서 다음 명령을 실행하여 키를 생성합니다. 여기서 "your_email@example.com"은 본인의 이메일 주소로 대체하세요.

   ssh-keygen -t ed25519 -C "your_email@example.com"

   이 명령은 새로운 Ed25519 SSH 키를 생성하고 이메일 주소를 주석으로 추가합니다. 엔터 키를 누르면 키 파일이 기본 디렉토리인 `~/.ssh/`에 저장됩니다.

2. **SSH 키 추가**: 이제 생성한 SSH 키를 SSH 에이전트에 추가해야 합니다. 에이전트를 실행하여 키를 추가합니다. 아래 명령을 실행하세요:

   eval "$(ssh-agent -s)"
   ssh-add ~/.ssh/id_ed25519

   이렇게 하면 SSH 키가 에이전트에 추가되고 사용할 준비가 됩니다.

3. **SSH 공개 키 복사**: 이제 SSH 공개 키를 복사하여 GitHub에 추가해야 합니다. 아래 명령을 실행하여 SSH 공개 키를 터미널에서 출력하세요:

   cat ~/.ssh/id_ed25519.pub

4. **GitHub에 공개 키 추가**:
   - GitHub 웹사이트에 로그인하세요.
   - 오른쪽 상단에 있는 프로필 아이콘을 클릭한 다음 "Settings"로 이동하세요.
   - 왼쪽 메뉴에서 "SSH and GPG keys"를 선택하세요.
   - "New SSH key" 또는 "Add SSH key" 버튼을 클릭하세요.
   - "Title"에 SSH 키에 대한 설명을 입력하고, "Key"에 앞서 복사한 SSH 공개 키를 붙여넣으세요.
   - "Add SSH key" 버튼을 클릭하여 키를 GitHub 계정에 추가합니다.

새로운 SSH 키가 GitHub 계정에 추가되었고, 이제 GitHub 리포지토리에 대한 SSH 액세스 권한을 사용할 수 있게 됩니다. 이렇게 하면 SSH를 통해 GitHub 리포지토리를 클론하고 작업할 수 있습니다.
