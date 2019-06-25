# APNs 서버 인증 방식
 - 인증서 : .p12인증서는 1년에 한 번씩 갱신 필요.
 - 인증키 : .p8키는 갱신 불필요.

# FushMessage 수신
 - AppDelegate.swift 수정
   - [FCM 공식 github](https://github.com/firebase/quickstart-ios/blob/a01a0aaf2aca46328582fdcda2cdb81112699a47/messaging/MessagingExampleSwift/AppDelegate.swift#L62-L97)
 - APP이 백그라운드에 있을 경우는 Push가 잘 오지만 포그라운드에서는 Push가 오지 않는 현상이 생김.
 - 예제소스에 몇 가지 코드를 추가해주니 잘 동작함.


 
