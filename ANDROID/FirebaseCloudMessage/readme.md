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
      - 추가시 app수준의 Gradle이
      dependencies {
          implementation fileTree(dir: 'libs', include: ['*.jar'])
          implementation 'com.android.support:appcompat-v7:28.0.0'
          implementation 'com.android.support.constraint:constraint-layout:1.1.3'
          testImplementation 'junit:junit:4.12'
          androidTestImplementation 'com.android.support.test:runner:1.0.2'
          androidTestImplementation 'com.android.support.test.espresso:espresso-core:3.0.2' 
      }
      이렇게 설정 되어 있는데
      
      dependencies {
          implementation fileTree(dir: 'libs', include: ['*.jar'])
          implementation 'com.android.support:appcompat-v7:28.0.0'
          implementation 'com.android.support:customtabs:28.0.0'
          implementation 'com.android.support:support-vector-drawable:28.0.0'
          implementation 'com.android.support:support-media-compat:28.0.0'
          implementation 'com.android.support:support-v4:28.0.0'
          implementation 'com.android.support.constraint:constraint-layout:1.1.3'
          testImplementation 'junit:junit:4.12'
          androidTestImplementation 'com.android.support.test:runner:1.0.2'
          androidTestImplementation 'com.android.support.test.espresso:espresso-core:3.0.2'
          //Add Line
          implementation 'com.google.firebase:firebase-core:16.0.1'
      }
      
      이렇게 바꿔줘야 에러가 나지 
