# git 설치 방법

## 1&#41; git 설치여부 확인
1. window키 + R 키로 실행 창 띄우기
2. cmd 라고 검색 후 cmd창 열기
3. cmd창에서 git --version 입력하여 깃 설치여부 확인

## 2&#41; git  설치하기
1. https://git-scm.com/ 에서 git download (setup파일에서 설정없이 쭉 next > install > finish)
2. cmd창 재부팅 후 설치여부 확인
3. git 버전이 나오면 설치 완료되어 사용할 수 있음

# github 연동하기
## 1&#41; vscode에 있는 코드를 github에 연동시키는 경우
### - Local에 프로젝트 커밋하기
1. 깃허브(https://github.com/) 회원가입 및 로그인 <br>
(name 입력 시 영어 닉네임으로 입력 ㅊㅊ)
1. vscode로 작업 중인 프로젝트 열기
2. 상단메뉴 > 터미널 > 새터미널 로 새터미널창 열기
3. 현재 프로젝트 경로가 맞는지 확인 
4. git --version 입력해서 깃 사용할 수 있는지 확인 
5. git init 입력으로 버전관리 선언 <br>
   6-1. vscode 왼쪽 하단에 master 라고 표시되는지 확인<br>
   6-2. 확인 안될 시 좌측메뉴 3번째 아이콘 클릭 후 새로고침
6. git config --global --list 입력하여 현재 연동된 깃허브 계정정보 있는지 확인<br>
   7-1. 없을 경우<br>
   - git config --global core.autocrlf true
   - git config --global user.name '깃헙 가입 시 입력한 name'
   - git config --global user.email '깃헙 가입 시 입력한 email'
   - git config --global --list 입력하여 등록정보 확인
7. git status 입력하여 현재 프로젝트 구조 확인
8. git add . 입력하여 status에 올림
9.  git commit -m '커밋메시지 입력' 하여 local에 프로젝트 버전 커밋
10. git log 입력하여 커밋되었는지 확인

### - Github에 저장소 만들기
1. github 홈페이지 접속 후 New 버튼 눌러서 Repository 생성
2. 연결할 저장소 주소 복사 

### - Github 저장소에 프로젝트 올리기
1. git remote add origin 복사한 저장소 주소 입력
2. git push origin master 입력하여 master 브랜치에 업로드<br>
(인증절차 있으면 완료 후 업로드 하세용)
3. github 접속해서 업로드 되었는지 확인




## 2&#41; github에 있는 코드를 local에 불러오는 경우
1. vscode 새창 열기
2. 모든명령표시(ctrl+shift+p)에서 git:clone 입력
3. github 접속 후 해당 repository 주소 복사하여 입력
4. repository 복제할 폴더 선택한 후 프로젝트 열기
  
