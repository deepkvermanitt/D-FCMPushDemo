# D-FCMPushDemo
This is a basic demo app that shows how to use Firebase Cloud Messaging (FCM) in an Android project built with Jetpack Compose and Kotlin. It helps you understand how to receive push notifications when the app is open, in the background, or even when it's closed — and how to handle what happens when a user taps on a notification.

**Sending Push Notifications**
Via **Firebase Console**
-->Go to Firebase Console
-->Navigate to Cloud Messaging
-->Paste the FCM device token shown in your app log
-->Enter the title and body for the test message
-->Send the message to test push notification handling
 
 **cURL (Command Line Tool)**

 Open terminal and run the following command:
 curl -X POST -H "Authorization: key=YOUR_SERVER_KEY" \
-H "Content-Type: application/json" \
-d '{
  "to": "YOUR_FCM_DEVICE_TOKEN",
  "notification": {
    "title": "Test Notification",
    "body": "This is a test message."

  }
}' https://fcm.googleapis.com/fcm/send 


**Replace** YOUR_SERVER_KEY with your **Firebase Server Key**
(Found in Firebase Console → Project Settings → Cloud Messaging tab)

**Replace** YOUR_FCM_DEVICE_TOKEN with the **device token printed** in your app log

This project follows MVVM with a clean architecture approach, making the FCM implementation modular, testable, and easy to scale — whether you're adding background sync, 
deep linking, or analytics in the future

<img width="432" height="488" alt="Screenshot 2025-07-20 at 3 32 37 PM" src="https://github.com/user-attachments/assets/30340eef-6f21-4d9f-a1fb-17ace45b9b73" />

 
