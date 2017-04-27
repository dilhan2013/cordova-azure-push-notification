**This document is not complete yet**

# Push notifications using Cordova and Azure Notification Hub

Goal of this document is to provide information required to implement cross platform (iOS, Android and Windows) push notifications using Cordova and Azure notification hub without requiring Azure mobile serivce client.

What you will need?
- Azure account (Using azure free account you can send up to 1 million push notifications. See pricing details [here](https://azure.microsoft.com/en-au/pricing/details/notification-hubs/))
- [Cordova phone gap plugin](https://github.com/phonegap/phonegap-plugin-push)
- Your cordova application
- Your backend Api (We will call Azure REST APIs from our backend service to register and unregister devices with Azure Notification Hub)

## Auzre notification hub
