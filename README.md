## 1. Deployment URL
  https://github.com/hachanghyun/chatApp
  
## 2. Summary
### 주요 기능
     (1). 회원가입 기능 (사진등록 및 변경)
     IOS는 실제 제 아이폰으로 테스트를 진행하였으며 Android는 시뮬레이터를 이용하여 테스트를 진행하였습니다. 
     각 플랫폼 별 회원가입 화면입니다. (왼쪽 : 아이폰, 오른쪽 : 안드로이드)
  ![시연7](https://github.com/hachanghyun/chatApp/assets/33058284/9dbe42d7-a40c-4168-bc69-cde53bb50b84)

     (2). 로그인 기능
     각 플랫폼별 로그인 화면입니다. 
    화면 상단에 있는 로고는 혹시 배포를 하게됬을때 저작권 방지로 직접 그린 로고입니다.
  ![시연6](https://github.com/hachanghyun/chatApp/assets/33058284/9cfb75ae-62e1-407d-b69d-7edfaaa826d8)

     (3). 채팅방 등록 기능
         로그인 후 채팅방 등록하는 화면입니다. 
   ![시연5](https://github.com/hachanghyun/chatApp/assets/33058284/09d218e0-54e1-47c6-9fc9-7e0685ff7ca0)
![시연4](https://github.com/hachanghyun/chatApp/assets/33058284/4e86202d-1588-4185-9516-70cf9da571d5)
     (4). 채팅 기능 
     채팅방에서 채팅하는 화면입니다. (아이폰 : bear@naver.com 로 로그인, 안드로이드 : rabbit@naver.com로 로그인)
![시연3](https://github.com/hachanghyun/chatApp/assets/33058284/e5beede3-0ecb-41df-85ec-065ad8664361)
![시연2](https://github.com/hachanghyun/chatApp/assets/33058284/5a61242e-5fe8-45e2-9570-60b1753642fb)

     (5). 프로필 조회 기능 
     접속한 계정 프로필 확인 화면입니다.
![시연1](https://github.com/hachanghyun/chatApp/assets/33058284/a342439e-2cce-4546-877b-c8c70d42588a)

     (6). firebase 
     앱에 필요한 로고와 사진 등록 프로필 사진을 firebase storage에 등록하였으며 읽기권한은 전체로 부여하였습니다.
     회원가입시 등록하는 사진은 각 계정별 uid 폴더밑에 경로로 저장시켯으며 프로필 읽기 권한은 전체, 프로필 쓰기 권한은 
     uid가 동일한 계정만 사용 가능하도록 설정하였습니다.
![firebase1](https://github.com/hachanghyun/chatApp/assets/33058284/1bae654b-172e-49f0-a898-d8c4d7a30eef)



    사용자 회원가입시 등록되는 사용자 권한 페이지이며 사용자가 등록될때마다 고유한 PK값 uid를 부여하였습니다.
 ![firebase2](https://github.com/hachanghyun/chatApp/assets/33058284/4f2a2506-033f-4e8b-a1da-356951d5476d)

    로그인한 사용자만 읽고 쓸수 있도록 DB channel(채팅방) 생성 권한을 등록하였습니다.
 ![firebase4](https://github.com/hachanghyun/chatApp/assets/33058284/de4580d9-abb9-438a-94af-1822c9f87441)

     사용자가 채팅방 정보를 등록하면 생성일자, 채팅방id(uid), 채팅방명(title)이 firebase database 에 등록됩니다.
![firebase3](https://github.com/hachanghyun/chatApp/assets/33058284/669431f8-c250-41b4-9210-b5c156d2e4d8)

     사용자가 채팅을 입력하면 채팅정보값(채팅uid), 생성날짜, 텍스트정보, 유저uid, 유저프로필사진(firebase storage에서 불러옴), 사명자명이 
     firebase database에 저장됩니다.
<img width="1033" alt="화면 캡처 2023-08-28 220900" src="https://github.com/hachanghyun/chatApp/assets/33058284/d1a78cb0-aa55-4659-8468-1f66a01669a4">

## 3. Meaning
    채팅앱을 예전부터 만들어보고 싶어서 인프런의 "처음 배우는 리액트 네이티브" 강의를 수강하여 듣게 되었습니다. 
    실제 앱개발이 처음이라 expo로 손쉽게 만들수있을것이라는 생각과 함께 시작했던 프로젝트가 정말로 힘든 프로젝트가 되었던 것 같습니다.
    기존에 Javascript를 안다고 자만했던 제 자신을 반성하며 앱 개발이 백엔드개발 만큼이나 이렇게 힘들다는것을 몸소 느끼게 되었습니다.

    이번 채팅앱은 정말 힘들게 만든만큼 배포까지가 목표였습니다. (IOS 개발자등록 1년에 $100, 구글 개발자 등록 $25  total= $125를 결재 하였습니다...ㅠㅠ)
    하지만 커뮤니티앱을 올리는만큼 관리부분(언어폭력 차단 방안)에 문제가 많을것으로 예상되어 배포는 하지 않게되었습니다.
    
## 4. Technology Stack(s)
    Frontend : Javascript, Native Cli, Expo
    
    Backend : Firebase Authentication
    
    Database : Firebase Database (Cloud Firestore)

## 5. Environment Setup

#### expo-cli 전역으로 설치해주는 명령어
    npm install -g expo-cli 

#### expo 프로젝트 만들어주는 명령어
    expo init "프로젝트명"
    
#### expo 프로젝트 실행
    npm init

#### node_module 설치
  npm install

#### eas 세팅 
    npm install -g eas-cli

#### log in expo accout
    eas login

#### configure the project
    eas build:configure
#### expo 프로젝트 실행
    npx expo start 
    npm start 
    
#### 빌드전 실행
    npm install -g eas-cli

#### IOS 빌드
    eas build -p ios

#### 안드로이드 빌드
    eas build -p android

#### styled components 라이브러리 추가
    npm i styled-components 

#### prop-types, react-navigation 라이브러리 추가
    npm I prop-types @react-navigation/native

#### (위에꺼 안되면) 리액트 네비게이션 라이브러리 설치
    npx expo install react-native-screens react-native-safe-area-context

#### 스택네비게이션 라이브러리 설치
    npm i @react-navigation/stack

#### 키보드가 화면 가리는현상 라이브러리 
    npm i react-native-keyboard-aware-scroll-view

#### 사진 picker 라이브러리
    expo install expo-image-picker

#### 경로 바뀌었을때 캐쉬 클리어
    npm start --clean-cache

## 6. 리액트 네이티브 내용 및 라이브러리

### 컴포넌트와 API
#### Alert
##### https://reactnative.dev/docs/alert

#### ActivityIndicator (spinner)
##### https://reactnative.dev/docs/activityindicator

#### FlatList (button selectable)
##### https://reactnative.dev/docs/flatlist

  

### 라이브러리
#### React Navigation (화면간 이동)
##### https://reactnavigation.org/

#### expo-image-picker (Device 사진첩 불러오기 라이브러리)
##### https://docs.expo.io/versions/latest/sdk/imagepicker/
    
#### expo/vector-icon 
##### https://docs.expo.io/guides/icons/
    
#### firebase 
##### https://docs.expo.io/guides/using-firebase/

#### react-native-keyboard-aware-scroll-view (keyboard에 화면 가려질때 스크롤 올라가는 기능 )
##### https://github.com/APSL/react-native-keyboard-aware-scroll-view

#### moment (날짜 타입 라이브러리)
##### https://momentjs.com/

#### react-native-gifted-chat (채팅 기능 라이브러리)
##### https://github.com/FaridSafi/react-native-gifted-chat

### 설치 세팅 

#### nvm 설치 
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash

      Running either of the above commands downloads a script and runs it. The script clones the nvm repository to ~/.nvm, and attempts to add the source lines from the snippet below to the correct profile file (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc).

      현재 zshrc 버전으로 update 되었음.
      vim ~/.zshrc

      export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm

    이거 소스 띄워쓰기 잘해야함 '[-s' 부분시작지점으로 해야함 이것때문에 30분 삽질함

#### nvm 명령어
    nvm help 

#### nvm 14버전 설치 명령어
    nvm install 14

#### 현재 설치되어있는 노드버젼 전부확인 
    nvm ls

### 안드로이드 에뮬레이터 세팅

#### jdk 11 설치
  brew tap homebrew/cask-versions
  brew install --cask zulu11

#### 자바 mac 에서 환경변수 설정 
    vim ~/.zshrc
    JAVA_HOME=/Library/Java/JavaVirtualMachines/zulu-11.jdk/Contents/Home
    PATH=$PATH:$JAVA_HOME/bin
    export JAVA_HOME
    export PATH
    
#### 소스 입력 확인
    source ~/.zshrc

#### 잘 적용되었는지 확인
     echo $JAVA_HOME

#### 안드로이드 스튜디오 sdk 세팅 arm은 applechip 으로 보면됨
<img width="455" alt="스크린샷 2023-08-15 오후 11 53 58" src="https://github.com/hachanghyun/chatApp/assets/33058284/468f509d-f597-4173-bb01-7ca08096ec2a">

#### ~/.zshrc 파일에 안드로이드 환경변수 등록
    export ANDROID_HOME=$HOME/Library/Android/sdk
    export PATH=$PATH:$ANDROID_HOME/emulator
    export PATH=$PATH:$ANDROID_HOME/platform-tools
