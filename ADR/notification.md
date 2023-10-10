# ADR University network app

* Decision title: Push Notification service collection 

* Status: Accepted 

* Deciders: Stadium Nay

* Date: 2023-10-07


* Context and Problem Statement:
The objective is to integrate the university networking mobile app with a notification service that supports IOS and Android platforms. The notification service should provide reliability and ease of integration with React Native. 

* Considered Options:

[1] APNs and FCM combination 
[2] Firebase Cloud Messaging (FCM)
[3] Amazon Simple Notification Service (SNS)
[4] OneSignal
[5] Pusher

* Decision:
The chosen push notification service for the university networking mobile app will be Firebase Cloud Messaging(FCM). It provides reliable cross-platform support for IOS and Android. Also, its integration with React Native makes it more suitable for sending out notifications to users effectively. 

* Rationale:
FCM supports both IOS and Android, ensuring that all users regardless of the device will reach out through notification. 

FCM works well with React Native, it simplifies the development process.

FCM has a great record of being a reliable and widely adopted push notification service.

FCM can handle notifications for a large user base, making it more efficient and suitable for university networking apps. 


* Consequences:
Since proper setup and configuration are essential for the push notification server to work, the team has carefully set up and made sure that the FCM is configured properly. 

Constantly monitoring and managing the cost of using FCM, especially for large base users.

Some platform-specific feature notifications might not supported by FCM fully. 

* Follow-Up Action:

The development team will be responsible for configuring FCM and integration of the app codebase.

Rigorous testing will be conducted to ensure proper push notification delivery for IOS and Android devices. 

The management team will monitor the cost that is associated with the FCM usage.

The development team will assess and implement any specific platform features that are required. 

Following this action will ensure that push notifications are effectively delivered to users. 


