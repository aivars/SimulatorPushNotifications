# Test project for simulator push notification tests

### How to video: https://youtu.be/zrpgzfmKZ7U

<img width="992" alt="Screenshot 2020-02-07 at 13 14 40 (2)" src="https://user-images.githubusercontent.com/774359/74028591-66269680-49b3-11ea-8059-726d6b87beeb.png">


Xcode 11.4 introduced push notification sending to the iOS simulator.
There is two ways hot to send them:
1) by sending them from the terminal
2) simple drag and drop APNS file to the simulator

apns file example : https://github.com/aivars/SimulatorPushNotifications/blob/master/test.apns
Download and save on Desktop or create new file *.apns 

Terminal command to send push notification: `xcrun simctl push <Device>  com.aivarsmeijers.pushNotifications test.apns`

<Device> should be replaced with used simulator id.
Simulator ID can be found using following terminal commands:
1) `xcrun simctl list`
2) `instruments -s devices`

Second works the best for me 
