# Advagym Puck Scanner


To integrate Advagym Puck Detection you will drag and drop 1 or 2 files to your project.

To Detect iBeacon we need Location Services Permission from user by adding this key to **info.plist** file with some text explaining why we need the permission

`NSLocationWhenInUseUsageDescription`

**Note:**
Chances are that you already have this key in info.plist file if you're app already uses location services


To Detect Advagym Puck all you have to do is call the ranging function:

`AGLocationManager.shared.startRanging()`

AGLocationManager will start ranging for Advagym puck as soon as it comes in contact with the puck it will check if Advagym App is already installed it will open the Advagym App else it will open App store.

To stop ranging beacon call:

`AGLocationManager.shared.stopRanging()`
