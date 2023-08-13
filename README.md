## 1. Deployment URL
  https://github.com/hachanghyun/chatApp
  
## 2. Summary
### 주요 기능
  
## 3. Meaning
    채팅앱을 예전부터 만들어보고 싶어서 인프런의 처음 배우는 리액트 네이티브 강의를 수강하여 듣게 되었습니다. 
  
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
    npx expo start 
    
    npm start 

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

#### 빌드전 실행
    npm install -g eas-cli

#### IOS 빌드
    eas build -p ios

#### 안드로이드 빌드
    eas build -p android
