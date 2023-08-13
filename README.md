## 1. Deployment URL
  https://github.com/hachanghyun/chatApp
  
## 2. Summary
### 주요 기능
     1.회원가입 기능
  ![시연7](https://github.com/hachanghyun/chatApp/assets/33058284/789fa641-fa5e-4ed6-a2b6-0c24f4dbc663)
     IOS는 실제 제 아이폰으로 테스트를 진행하였으며 Android는 시뮬레이터를 이용하여 테스트를 진행하였습니다. 
     각 플랫폼 별 화면입니다. (왼쪽 : 아이폰, 오른쪽 : 안드로이드)
         

     2.로그인 기능 (사진등록 및 변경)
     
     3.채팅방 등록 기능
     
     4.채팅 기능 
     
     5.프로필 조회 기능 
     
## 3. Meaning
    채팅앱을 예전부터 만들어보고 싶어서 인프런의 "처음 배우는 리액트 네이티브" 강의를 수강하여 듣게 되었습니다. 
  
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
