**This document is not complete yet**

# Push notifications using Cordova and Azure Notification Hub

Goal of this document is to provide information required to implement cross platform (iOS, Android and Windows) push notifications using Cordova and Azure notification hub without requiring Azure mobile serivce client.

What you will need?
- Azure account (Using azure free account you can send up to 1 million push notifications. See pricing details [here](https://azure.microsoft.com/en-au/pricing/details/notification-hubs/))
- [Cordova push plugin](https://github.com/phonegap/phonegap-plugin-push)
- Your cordova application
- Your backend Api (We will call Azure REST APIs from our backend service to register and unregister devices with Azure Notification Hub)

## Auzre notification hub
Configure Windows, Goole and Apple notification hubs using the portal

### Apple Push Notifications
You have to use development certificate when testing and switch to production certificate when the app is deployed to App store.
Note: Same notification certificate will not work in both dev and production environment

## Debug Azure notification hubs

Notification hubs can be viewed using Visual Studio or using Service Bus Explorer. [This link](https://msdn.microsoft.com/en-us/library/azure/dn530751.aspx) has more information.

## Some Tips 
You have to handle the notification in following senarios,
- Notification received while app is in background
- Notification received while app is running in forground (when the user currently working in the app)
- Notification received while app is not running (not even in background)

