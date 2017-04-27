**This document is not complete yet**

# Push notifications using Cordova and Azure Push Notification Hub

Goal of this document is to provide information required to implement cross platform (iOS, Android and Windows) push notifications using Cordova and Azure notifications hub without requiring Azure mobile serivce client.

What you will need?
- Azure account (Using azure free account you can send up to 1 million push notifications)
- cordova phone gap plugin
- Cordova application
- Some changes to your backend Api (We will call Azure REST Apis to register, unregister devices with Azure push notification hub)
