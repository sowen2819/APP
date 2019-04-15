# 명칭

  - C2DM -> GCM -> FCM으로 명칭 변경
  
# 필요 요소
  
  - Gradle
  - FirebaseMessaging API
  - Android Studio 1.4 이상
  - Android 4.1(Jelly Bean) : API 16 이상
  - [FCM 홈페이지](https://firebase.google.com/docs/cloud-messaging/android/client)

# 설정 방법
  
  1. [console](https://console.firebase.google.com/) 접속
  2. 프로젝트 추가
  3. Android 앱에 Firebase 추가
  4. Android 패키지 이름 ( com.example.fcmtest ) 추가
  5. 앱등록
  6. google-services.json 다운  
  
  ------여기서부터는 FCM console을 따라 구현------
  
  7. Android Studio 실행
  8. Project 선택
  9. FirebaseCloudMessage/app/에 google-services.json 추가 [ FirebaseCloudMessage/app/google-services.json ]
  10. gradle에 FCM_lib추가
