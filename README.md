# pbi_home 작업 일지 

1일차 : 

<깃 허브로 웹 사이트 만들기>

1.새 리포지터리 만들기 : 이름이 중요해요!.
GitHub 우측 상단 + 버튼 ➔ New repository를 누르고 아래 규칙대로 이름을 지어줍니다.
  Repository name: 내_계정이름.github.io로 입력해야 합니다. (예: 내 계정 아이디가 gildong이라면 gildong.github.io)
  Public/Private: 반드시 **Public(공개)**으로 설정해야 웹 사이트가 외부로 노출됩니다.
  
2.index.html 파일 업로드하기 : 첫 페이지 만들기.
생성된 리포지터리에 웹 사이트의 메인 화면이 될 파일을 올려야 합니다.
  반드시 파일 이름이 소문자 **index.html**이어야 시스템이 첫 페이지로 인식합니다.
  웹화면에서 Add file ➔ Create new file을 눌러 간단히 테스트용 코드를 적고 저장(Commit)해 보세요.

3.GitHub Pages 활성화 확인 : 설정 켜기.
주소를 계정명 규칙(계정명.github.io)으로 만들었다면 자동으로 배포가 시작되지만, 확인을 위해 설정으로 이동합니다.
  1) 리포지터리 상단의 Settings (톱니바퀴)를 누릅니다.
  2) 좌측 메뉴에서 Pages를 클릭합니다.
  3) Build and deployment의 Branch가 main (또는 master)으로 잘 지정되어 있는지 확인합니다.

4.나만의 웹 사이트 주소로 접속 : 접속하기.
상단에 "Your site is live at..." 이라는 메시지와 함께 링크가 나타납니다.
이제 전 세계 어디서든 https://내_계정이름.github.io 주소로 접속하면 내가 만든 웹 사이트가 뜨는 것을 볼 수 있습니다! (반영되는데 1~2분 정도 걸릴 수 있습니다.)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
알아두면 좋은 팁
일반 리포지터리 이름으로도 만들 수 있나요?
네, 가능합니다! 리포지터리 이름을 일반 프로젝트명(예: my-portfolio)으로 만들고 Settings ➔ Pages에서 브랜치를 켜주면, https://내_계정이름.github.io/my-portfolio/ 라는 주소로 웹 사이트가 생성됩니다. 하나의 계정으로 여러 개의 웹 사이트를 만들 때 유용합니다.

개인 도메인 연결 가능
goDaddy나 가비아 같은 곳에서 따로 구매한 개인 도메인(예: [www.myname.com](https://www.myname.com))이 있다면, 이 무료 GitHub Pages에 연결해서 사용할 수도 있습니다.

제한 사항
GitHub Pages는 정적(Static) 웹 사이트만 지원합니다. 즉, HTML/CSS/JS로 이루어진 포트폴리오, 블로그, 소개 페이지는 완벽하게 작동하지만, Node.js나 Python(Django), 데이터베이스(MySQL)가 필요한 로그인 기능, 회원가입 기능 등은 작동하지 않습니다.

------------------------------------------------------------------------------------------------------------------------------------------------------------------

<리포지터리 복사 및 업로드>

기존 리포지터리의 소스 코드 파일들을 내 컴퓨터로 다운로드(복사)한 뒤, 완전히 새로운 리포지터리를 만들어 그대로 업로드하는 방법입니다.

커밋 히스토리(과거 기록)를 다 버리고, "현재 기준의 순수 소스 코드 파일만 깔끔하게 복사해서 새로 올리고 싶을 때" 가장 많이 쓰는 방법이에요.

터미널이나 명령어를 쓰지 않고 GitHub 웹사이트 화면에서 마우스 클릭과 압축 풀기만으로 해결하는 방법이 가장 쉽습니다. 그대로 따라 해보세요!

1단계: 기존 리포지터리 소스 전체 복사 (다운로드)

<img width="404" height="247" alt="image" src="https://github.com/user-attachments/assets/07a1ffb6-6d57-401c-aec8-f2e7065e9072" />

1. 복사하고 싶은 기존 GitHub 리포지터리 페이지로 이동합니다.
2. 위 이미지처럼 우측 상단에 있는 초록색 Code (또는 Clone or download) 버튼을 클릭합니다.
3. 드롭다운 메뉴 맨 아래에 있는 Download ZIP을 누릅니다.
4. 내 컴퓨터에 다운로드된 압축 파일(.zip)을 찾아서 압축을 풀어줍니다. 이제 소스 코드 전체 복사는 끝났습니다!

2단계: 새로 업로드할 빈 리포지터리 만들기
1. GitHub 우측 상단의 + 아이콘을 누르고 New repository를 클릭합니다.
2. Repository name에 새로운 저장소 이름을 적어줍니다.
3. [중요] 아래 초기화 옵션(Add a README file, .gitignore, License)은 모두 체크 해제(빈 상태)로 둡니다. 아무것도 없는 순수 빈 방이어야 파일 업로드가 쉽습니다.
4. 맨 아래 Create repository 버튼을 누릅니다.

3단계: 소스 파일 통째로 업로드하기
READ.ME 파일을 만들지 않고 빈 저장소를 생성하면 화면 중앙에 파란색 글씨로 된 안내 문구들이 보입니다.
1. 안내 문구 중간 즈음에 있는 uploading an existing file 이라는 파란색 링크를 찾아서 클릭합니다. (또는 화면 상단 탭에서 Add file ➔ Upload files 선택)
2. 파일 업로드 창이 뜨면, 아까 1단계에서 압축을 풀어두었던 소스 코드 폴더 안의 모든 파일과 폴더를 전체 선택(Ctrl + A) 합니다.
3. 선택한 파일들을 마우스로 드래그해서 GitHub 웹 화면의 Drag files here... 영역에 떨어뜨려 줍니다.
4. 파일들이 쭉 업로드되는 것을 기다립니다.
5. 업로드가 완료되면 화면 아래 초록색 Commit changes 버튼을 누릅니다.

💡 주의할 점
만약 소스 코드 전체 파일 수가 100개가 넘거나, 단일 파일 크기가 너무 크다면 웹사이트 화면에서 드래그앤드롭으로 올릴 때 오류가 나거나 업로드가 제한될 수 있습니다.
파일 개수가 너무 많아 웹 업로드가 안 되는 경우에는, 아까 생성 직후 화면에 보였던 **Git 명령어(CLI)**를 터미널에 입력해서 올려야 합니다. 혹시 파일이 너무 많아 오류가 발생하면 말씀해 주세요. 터미널 명령어로 1초 만에 올리는 법을 다시 알려드릴게요!

----------------------------------------------------------------------------------------------------------------------------------------------------
2일차 :

#vibe01 MNIST CNN 손글씨로 숫자 입력하면 인식, 딥러닝

1. claude Code를 Vscode 에서 작업하기
2. 로컬 대상 폴더 지정 : d:\0.test\PBI0524
3. 클로저 코드 실행하고, 아래와 같은 프롬프트 활용 진행

(1단계) "손글씨로 숫자를 입력하면 이것을 인식하는 코드를 만들어서 실행해 줘. 모든 코드와 주석을 영어로 작성해 줘." 

<시스템 구조> 는 아래와 같이 나옴.
<Pre>
digit_recognizer.py
├── 1. CNN 모델 (build_model)
├── 2. 학습/로드 (load_or_train_model)
├── 3. 이미지 전처리 (preprocess_canvas_image)
└── 4. GUI 앱 (DigitRecognizerApp)
</Pre>

(2단계) "숫자 인식 프로그램을 윈도우 탐색기에서 클릭해서 실행할 수 있게 해 줘."

<완성된 파일 목록> 은 아래와 같이 나옴.
<pre>
digit_recognizer.py	메인 프로그램 (CNN + GUI)
digit_recognizer.bat	더블클릭 실행 파일
digit_recognizer.ico	앱 아이콘
mnist_model.keras	학습된 모델 (10 MB)
바탕화면 바로가기	손글씨 숫자 인식기.lnk
</pre>

(3단계) "/init" 

CLAUDE.md 파일 생성하는 명령어

(4단계) "#앞으로 만드는 모든 파일은 날짜와 시간을 주석으로 표시해 줘."

"#" 을 붙이고 명령어를 넣으면 CLAUDE.md 파일에 직접 넣을 수 있음

(5단계) "손글씨 인식 프로그램을 웹 버전과 데스크톱 버전으로 나누어 개발하고 싶어. web_version과 desktop_version 폴더를 만들고, 각 폴더에 해당하는 CLAUDE.md 파일도 생성해 줘."

웹 버전과 데스톱 버전으로 진행할 수 있도록 폴더별로 정리함.

<완성된 구조> 는 다음과 같음.
<pre>
pbi0524/
├── mnist_model.keras          ← 공유 모델 (두 버전이 함께 사용)
├── CLAUDE.md                  ← 루트 가이드 (업데이트됨)
│
├── desktop_version/
│   ├── digit_recognizer.py   ← Tkinter GUI 앱
│   ├── digit_recognizer.bat  ← 더블클릭 실행
│   ├── create_icon.py        ← 아이콘 생성
│   └── CLAUDE.md             ← 데스크톱 개발 가이드
│
└── web_version/
    ├── app.py                ← Flask 서버 (REST API)
    ├── run_web.bat           ← 더블클릭 실행
    ├── requirements.txt
    ├── templates/index.html  ← 드로잉 UI
    ├── static/css/style.css  ← Catppuccin 테마
    ├── static/js/app.js      ← 캔버스 + fetch 로직
    └── CLAUDE.md             ← 웹 개발 가이드
</pre>

(6단계) "아래 깃 연동해주고, 연동된 깃으로 web_version 이 업로드 될 수 있도록 해 줘. 업로드 후에는 깃을 이용하여 웹에서 실행시킬 수 있도록 준비해 줘.
깃 주소는 https://github.com/chpark20/vibe01.git
이메일은 chpark20@dankook.ac.kr 이야. "

이렇게 넣어주고 약간 후회함. 어떻게 배포해야 하는지 알려주지 않아서, Render 배포 파일 작성해 주었음. (https://render.com )
배포 방법은 깃허브 페이지 이용하는 방법, 버셀 이용하는 방법 이렇게 2가지를 연구함.

(7단계) "깃허브에 올려진 웹 버전 폴더를 버셀에 배포해 줘."
<pre>
Vercel 배포 순서 (웹 대시보드)
1단계 — Vercel 계정 생성 및 GitHub 연동

vercel.com → Sign Up → Continue with GitHub
GitHub 계정으로 로그인
2단계 — 새 프로젝트 추가

대시보드에서 Add New… → Project 클릭
chpark20/vibe01 저장소 옆 Import 클릭
3단계 — 프로젝트 설정 (중요!)

항목 : 값
Framework Preset	: Other
Root Directory :	web_version ← 반드시 변경
Build Command	 : (비워두기)
Output Directory : (비워두기)
Root Directory 옆 Edit 버튼 클릭 → web_version 입력
4단계 — Deploy 클릭

1~2분 후 https://vibe01-xxxx.vercel.app 주소가 생성됩니다
</pre>

(8단계) "깃허브 올려진 웹 버전 폴더를 깃허브 페이지를 이용하여 배포할 수 설정 해 줘."

<font color="#1e73be"> GitHub Pages는 정적 파일(HTML/CSS/JS)만 서비스하므로 Flask(Python 서버)를 그대로 올릴 수는 없습니다. 대신, ONNX Runtime Web을 사용해 모델 추론을 브라우저에서 직접 실행하는 순수 정적 버전으로 변환하면 GitHub Pages에 완벽하게 배포할 수 있습니다. 그래서, 파이썬이 들어가 있는 이 문서는 실패!!  </font>

<pre>
GitHub Pages 활성화 (마지막 단계)
1단계 — vibe01 저장소 Settings 열기

2단계 — Pages 설정에서:

항목	선택
Source	Deploy from a branch
Branch	main
Folder	/docs
→ Save 클릭

3단계 — 1~2분 후 배포 완료

URL: https://chpark20.github.io/vibe01/

    
지금 배포된 방식:

브라우저
  └─ index.html (docs/)
       ├─ onnxruntime-web CDN (jsdelivr)  ← ONNX 추론 엔진 (JS)
       ├─ mnist_model.onnx (3.3 MB)       ← 모델 다운로드
       └─ app.js                          ← 캔버스 + 전처리 + 추론 전부 브라우저에서 실행
서버가 전혀 필요 없이 브라우저 안에서 추론하므로 GitHub Pages (정적 호스팅)에서 완벽하게 동작합니다. Settings → Pages에서 /docs 폴더를 소스로 지정하면 바로 라이브됩니다!
</pre>
-----------------------------------------------------------------------------------------------------------------------------------
