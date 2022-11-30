# Wear OS watch app

You now can use you Wear OS watch to control your Cowboy bike via the [Untamed app](https://github.com/Imaginous/Cowboy_Untamed) *([V3.60 or up](https://github.com/Imaginous/Cowboy_Untamed/releases/latest))*.<br>
Unfortunately you cannot pair your bike directly to your watch, so the phone and Untamed app are always needed.

## Donate
If you like the instructions and watch app, you're welcome to make a [donation](https://github.com/Imaginous/Cowboy_Untamed/blob/main/README.md#donate). 

## Usage

You need to sideload the app onto your watch. 
For this you need to enable the developer options and use two ADB commands to upload the app to your watch.

#### Enabling developer options (Galaxy Watch 5)
Watch this YouTube video on enabling developer options: [Enable developer options](https://www.youtube.com/watch?v=i4VtRxtBLrM)

Once you have enabled the developer options on your watch and do the following:
- Go to settings
- Go to developer options
- Enable ADB-Debugging
- Enable debugging via WiFi and take **note** of the **IP address** shown.

**Note: disable ADB-debugging once the app is installed**. Otherwise your battery will be drained very fast.

#### Using ADB (windows)
Download the ADB-Tools from Google: [ADB-Tools](https://developer.android.com/studio/releases/platform-tools)

- Extract the contents to a known location (C:\temp)
- [Download the cowboyuntamed_watch_vx_xx.apk](https://github.com/Imaginous/Cowboy_Untamed/releases/latest) and place it in the folder: C:\temp\platform-tools
- Open a *command prompt (CLI)* as *administrator*
- Enter: CD C:\Temp\platform-tools
- Enter: adb connect **x.x.x.x**:5555 *(Replace x.x.x.x with the IP address noted earlier)*<br>
When you connect for the first time you must acknowledge that the current computer is allowed ADB access.
- Enter: adb install cowboyuntamed_watch_v**x_xx**.apk *(Replace x_xx with the version number of the file you have downloaded)*
- Enter: adb disconnect **x.x.x.x**:5555 *(Replace x.x.x.x with the IP address noted earlier)*
- Disable ADB on your watch in the developer settings 

Now the app should be installed. You must also activate the Watch service in the Untamed app on your phone. See next chapter.

Extra info on ADB: [Video](https://www.youtube.com/watch?v=WDboArbdFIo)

#### Activate in Untamed
In the Untamed app on your phone do the following:
- Go to the main menu *(in the upper right corner)*
- Go to *Settings*
- Enable *Start watch service on app launch*<br>**Please note: the watch app service is not yet started automatically**
- Go back
- Go to the main menu *(in the upper right corner)*
- Select *Start Watch Service*

The service will show a *watch* icon, you may hide/disable this notification.

#### Using the watch app
Now you can start the Untamed app on your watch. This will fetch the current options from the Untamed app on your phone.<br>
Once loaded it will show the *Actions*  menu.
- Slide an option button to the **right** to **enable** it.<br>Sliding *Power* to the *right* will turn *on* the bike.
- Slide an option button to the **left** to **disable** it.<br>Sliding *Power* to the *left* will turn *off* the bike.
- With the *...* button you can go to the main screen. Here you can select the *Presets* menu, or quit the app.

