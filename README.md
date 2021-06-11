# Cowboy Untamed
An Android app to lift the speed limit of your Cowboy bike and make other tweaks to make the bike even better.

## LEGAL NOTICE
#### !!! USE THIS APPLICATION AT YOUR OWN RISK
#### !!! I do not accept any liability.
#### !!! Unlocking your bike will make your bike illegal in most countries, atleast in the European Union.
#### !!! It might void your warranty

## Download
Direct download: [Cowboy Untamed V3.01](https://github.com/Imaginous/Cowboy_Untamed/releases/download/V3.01/cowboyuntamed_v3_01.apk)<br>
Version information: [Version overview](https://github.com/Imaginous/Cowboy_Untamed/releases)

## Donate
If you like the app you're free to make a small donation.<br>You can do this securely via [PayPal](https://paypal.me/pools/c/8zcWXI7VnO).<br>
If you have a Dutch bank account you may also make your [donation via iDeal](https://betaalverzoek.rabobank.nl/betaalverzoek/?id=EkJA4Zm7Qpq1eDSKdddMeQ).

## Free accessories on your new bike
If you don't have a Cowbow bike yet... use this [refferal link](https://share.cowboy.com/r/michelv3) for €100 of free accessories on your new bike.

## Introduction
*Main Features:*
- Disable speed limit of your Cowboy bike.
- Set field weakening to increase the maximum speed.
- Enable *Auto Unlock* on the V1+ model.
- Use shortcuts to unlock/lock your bike, turn on/off the lights. These can also be used in combination with the original Cowboy app and with automation apps like *Tasker*.
- *Set and forget*, just make the settings you want and start using the original Cowboy app again.

*Quick Launch Presets in V3.xx:*
- Quickly start your bike with one of three prefered settings without saving them to flash memory.
- Lower the default peddle to motor torque conversion. Lowering the assistance, making you work harder.
- Lower the maximum power output for given speed ranges. You can lower the power output for 10-20km/h so it's more easy to cycle along a non e-bike rider. But still have the punch to get going.


<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/119372390-8cab3680-bcb7-11eb-8d2c-c685640cb8ac.png" alt="Screenshot main app" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/119372491-a9e00500-bcb7-11eb-87df-e4dcc1d19b9b.png" alt="Screenshot expert page" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/121254562-b1ec9700-c8aa-11eb-9aaa-fff43845ab1b.png" alt="Screenshot quick launch presets" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/119372515-b2384000-bcb7-11eb-9b1a-633b93c2d93e.png" alt="Screenshot shortcuts main app" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/121254592-badd6880-c8aa-11eb-86db-a6b5ab1bea7f.png" alt="Screenshot shortcuts presets app" width="250"/>
</p>

This app is created as a hobby project. I love electronics and programming and just could not resist if I could get more out of my Cowboy V1+ bike.

This is where I started finding out how the Cowboy bikes work. Which electronics they use and how the electronics communicate internally and with the outside world.
I posted on [Reddit](https://www.reddit.com/r/cowboybikes/comments/m6zrdx/disable_speed_limit/) and it got more attention then I had anticipated.

So use this app to remove the speed limit and enjoy your Cowboy even more!

Special thanks go to Runereader for making his Bronco code open source.
This is my first Android app, pure hobby, so it is "as is".

## Installation
You must allow installation from unknown sources to install the Cowboy Untamed APK file.

- Goto `Settings` on your Android phone.
- Goto `Security`.
- Check the `Unknown Sources` option.

Now you should be able to download and install the APK file.<br><br>
For security reasons I recommend to disable this option after installing.<br><br>
**Note:** Since some users buy a second hand Android phone just to use this app, make sure you have Android version 7.1.1 or higher.

## Usage
This app can disable the speed limit of your Cowboy V1/2/3 bike.
For V1+ owners, you can now enable the 'Auto Unlock' function normally only available on V2 and V3 bikes.
When you only disable the speed limit you will be able to get up to 29km/h. At this point the motor magnetic field flux will start working against you.
You can overcome this effect by using field weakening.
A drawback of field weakening is the fact that it costs extra current, so your battery will be depleted faster.

I recommend a field weakening value of 15%. More then 20% would be inefficient and might cause damage to the motor. ASI advices a maximum of 25%, therefore the app is limited to 25%.

- **Make sure the original Cowboy app has been closed completely (and apps like Bronco).**
- No other devices may be connected via bluetooth to your bike.
- Make sure you only have one bluetooth profile called "Cowboy" and that this is the correct bike.<br>Multiple bikes are not (yet) supported.
- Make sure you are close to your bike.
- Open the Cowboy untamed app.
- Slide the connect switch to the "on" position.
- Wait patiently for the app to connect.
- The other options will be enabled after the connection is established. The current values will be read from the bike.
- Your first time... take a note of the current settings to undo them later.
- Select Torque (no speed limit) - If you want to disable the speed limit.
- On the line enter the wanted field weakening value, lets say 15.
- Press the "TEST" button. The values will be send to your bike. You can ride the bike to test the settings.<br>Please note that once the bike is locked or the battery is removed the settings will be lost at this stage.
- If you are satisfied you have to store the values "permanently" into the flash memory of the motor controller<br>Press the "FLASH" button to do this.
- Move the connection slider back to the off position. The app will lock the bike and disconnect.
- Now you are done. You can start using your bike like you did before. You can use the original Cowboy app.

##### Restoring default settings
Use the same method as above, but entering the values you have written down on first use.
Alternative method using my hardcoded defaults, unlock following the above mentioned procedure.
- Connect to the bike.
- Press the "DEFAULTS" button to fill in the default settings.
- Press the "TEST" button to send them to the bike.
- Press the "FLASH" button to store them in the flash memory of the motor controller.
- Disconnect from the bike.

#### Quick Launch Presets
With this new feature (and second app icon) you can setup three presets (Slow, Normal, Fast) and quickly unlock your bike with one of these presets. Just long press the *Cowboy Untamed Presets* app icon and select one of the three presets. Clicking the *Cowboy Untamed Presets* app icon will unlock the bike with the last used preset. These presets are not stored in flash and will be reset after locking your bike.<br><br>
**Note:** do not use the *FLASH* button in the main app while a preset is active. This will store the preset settings in flash memory.<br><br>
To configure the *Quick Launch Presets* go to the corresponding menu in the main app.<br><br>
As stated earlier I made some discoveries how to make the bike peddle a little bit heavier. Sometimes I find the default force a bit to low to my likings. With the *Quick Launch Presets* you can now alter the peddle torque to motor torque level. By decreasing the *Peddle Max Torque* percentage the overall force needed to power your Cowboy will be increased. 100% is default, lower values will make you sweat more.<br><br>
To get more precise control over the motor power the motor controller has 8 registers to set the maximum power output at certain speeds. These speeds are determined by the set maximum speed.<br>This is why you need to be connected to your bike when configuring. This will get the set maximum speed and calculates the corresponding speed ranges. These will be noted underneath each speed level.<br>
You can now set the maximum power as a percentage, 100% is default, 0% is no assist at all at the given speed range.<br>
With this system you can still get up to speed with 100% power, but when reaching 10km/h you can lower the output so you have to peddle harder. This makes it more natural when cycling along a non e-biker.<br><br>
Off course you can also set *field weakening*. When left empty the bike operates in its default mode (torque with speed limit). Entering 0-20% will disable the speed limit and set *field weakening*.<br><br>
At this point in time I can't give any advise on the "best" values. Just determine them with trail and error.<br><br>
**Note**: empty fields are not send to the bike. The default values stored in the motor controller are used. As stated before don't use the *FLASH* button in the main app when your bike was unlocked using a preset. First lock your bike then start the main app to do alterations. 


##### V1+ Headlight bug
A bug on the V1+ is a non working headlight, the taillight still works.<br>Can it be fixed? With the Cowboy Untamed app you can reset your PCB. This will not reset any settings but only reboot the communications PCB. 9 out of 10 times the headlight bug will be fixed (for a while). There is no fix from Cowboy yet.<br>Connect to your bike with the Cowboy Untamed app. Go to the *Expert Settings* and press the *Reset PCB* button. This will reboot the bike, shown by "running lights" on the main tube LEDs. 

##### My current favorite V1+ settings:
For me the sweetspot between excercise and still going fast came up with the following settings:
- Speed Limit: **Disabled** *(duh)*
- Field Weakening: **18**
- Peddle Max Torque: **85**

## The future
I think there is a quite solid base now for the future. Offcourse removing the speed limit was my main goal. Second I wanted to make shortcuts which I could use via *Tasker*.<br>I have discussed with other bikers and some of us would like to be able to set the support level. When you want to ride along with a non e-biker the support should be a lot less. The idea is to make speed dependant support. Let's say 0-10km/h you get the current support, 11-22km/h low to no support, 23->km/h regular untamed support. The levels can be set by the user. You can activate them via a long press shortcut.<br><br>These are ideas. I'm now ready to start exploring how to. I believe it can be done, but I want to do some serious testing with my own bike before I release it into the wild.<br><br>
**2021-05-29**: Finally some nice weather. I did some testing this morning. At his point I made the following discoveries:
- Adjusting various gain settings did not give me the hoped response. I can't feel a real difference when I suppress the torque and peddle gains. This might need further investigation. Since I think it would be the best option to a natural feel in cycling.
- The other thing, which is working as expected, is setting the 8 power levels. For certain speed ranges you can set the maximum power output as a percentage. Default Cowboy uses 100% for all 8 levels. I tried adjusting them and it works flawlessly. You can set the power output in 8 stages. So you can still have 100% power to get up to 6km/h. Then you can set it to 25% for 6-20 km/h. You have to work a lot harder, but will preserve battery and it's a more fair game between you and a non electrified biker ;) Then you can set it to 75% from 20 km/h and up for example.<br>The major drawback of this system is you might need more power when going uphill... you won't get it untill you drop below a certain speed.<br>Therefore a gain based reduction would be better, but I'm not getting any usefull results with that.

**2021-06-03**: i did some more research and testing. I found a second setting which is interesting. I can adjust the maximum voltage range of the torque sensor. By raising this you have to peddle harder (get less assistance). 
This setting can be handy to put in a bit more effort yourself and spare battery power. 

**2021-06-08**: A pre-release version of the *Quick launch Presets*.<br><br>The following whishes have popped up from users:
- *Walk* mode. A function where the bike propells its self at low speed. This can be handy when the belt has snapped. Technically it's possible via a hardware switch... now I have to figure out if it can be done by software only. It must be via an official function of the motor controller, because I don't want to do dirty hacks which can lead to failure or injuries.
- *Auto Unlock without the original Cowboy app*, some of you just want to grab the bike and ride. They don't need trip history, speed or what so ever. For this I need a background service which constantly scans for the bike. This must be done with an as low as possible battery usage. That part might be the biggest challenge.<br>This in combination with *auto unlock* and *auto lock* on the bike enabled could be handy for those users. 


## FAQ

- When I download the file, nothing happens?<br>The file has been downloaded in the background. Go to the upper right menu in *Chrome* and select *Downloads*. Now select the file and install it.<br>You can also use a tool like *CX File Explorer* to goto your downloads and install it.
- Will there be an IOS version?<br>No, unfortunately I do not have (and have no intention to) an Apple developers account.<br>But you can do it manually, see: [IOS.md](https://github.com/Imaginous/Cowboy_Untamed/blob/main/IOS.md).
- Why should I enter 15% or 18% for the field weakening values?<br>These are merely my advise. The lower you keep the percentage the better it is for your battery range. At the moment I'm using 18% on my V1+ bike. It feels speedy enough, going faster makes my legs go round like a mad man. It's fun for a while, but not for a longer stretch. So 18% is my sweet spot. I assume on a V3 bike 15% is a more likely figure because of the lower gear ratio compared to the V1 and V2.
- Can the settings be undone?<br>Yes, if you have not tinkered with this app (or other apps like Bronco) you can write down your settings and re-apply them later. Using the defaults button can be tricky if Cowboy changes their default settings. Until now they didn't so you should be safe.
- I want to make a donation, how?<br>[Donate via PayPal](https://paypal.me/pools/c/8zcWXI7VnO)<br>If you have a Dutch bank account, [Donate via iDeal](https://betaalverzoek.rabobank.nl/betaalverzoek/?id=EkJA4Zm7Qpq1eDSKdddMeQ).
- Can I use another Android phone to make the settings?<br>Yes, you can use a different Android phone to make the settings and then switch back to your original phone. This can also be an iPhone. Also auto unlock should work with a V1+ and an iPhone.
- Will this app work on a Cowboy V4?<br>I really don't know. I have not seen the bike in real life. If somebody can lent me one for a day I can probably find out if it is possible.<br><br>I assume the use another motor controller because of the more powerfull motor. But if they stayed with ASI they might have used an BAC500. This one is compatible with my app. But I also think they have changed the communications controller. Probably located in the handlebar console.<br><br>But this is all guessing, have to go hands on with the bike to make hard claims.
