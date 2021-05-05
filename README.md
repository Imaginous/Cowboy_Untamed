# Cowboy Untamed
An Android app to lift the speed limit of your Cowboy bike and make other tweaks to make the bike even better.

## LEGAL NOTICE
#### !!! USE THIS APPLICATION AT YOUR OWN RISK
#### !!! I do not accept any liability.
#### !!! Unlocking your bike will make your bike illegal in most countries, atleast in the European Union.
#### !!! It might void your warranty

## Introduction
This app is created as a hobby project. I love electronics and programming and just could not resist if I could get more out of my Cowboy V1+ bike.

This is where I started finding out how the Cowboy bikes work. which electronics they use and how they communicate internally and with the outside world.
I posted on Reddit and it got more attention then I had anticipated.

Special thanks go to Runereader for making his Bronco code open source.
This is my first Android app, pure hobby, so it is "as is".

## Usage
This app can disable the speed limit of your Cowboy V1/2/3 bike.
When you only disable the speed limit you will be able to get up to 29km/h. At this point the motor magnetic field flux will start working against you.
You can overcome this effect by using field weakening.
A drawback of field weakening is the fact that it costs extra current, so your battery will be depleted faster.

I recommend a field weakening value of 15%. More then 20% would be inefficient and might cause damage to the motor. ASI advices a maximum of 25%, therefore the app is limited to 25%.

##### Make sure the original Cowboy app has been closed completely (and apps like Bronco)

- No devices may be connected via bluetooth to your bike.
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


## FAQ

- Will there be an IOS version?<br>No, unfortunately I do not have (and have no intention to) an Apple developers account.
- Can the settings be undone?<br>Yes, if you have not tinkered with this app (or other apps like Bronco) you can write down your settings and re-apply them later. Using the defaults button can be tricky if Cowboy changes their default settings. Until now they didn't so you should be safe.
