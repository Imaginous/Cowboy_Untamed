# Cowboy Untamed
An Android app to lift the speed limit of your Cowboy bike and make other tweaks to make the bike even better.

## LEGAL NOTICE
#### !!! USE THIS APPLICATION AT YOUR OWN RISK
#### !!! I do not accept any liability.
#### !!! Unlocking your bike will make your bike illegal in most countries, atleast in the European Union.
#### !!! It might void your warranty

## Download
Direct download: [Cowboy Untamed V2.61](https://github.com/Imaginous/Cowboy_Untamed/releases/download/V2.61/cowboyuntamed_v2.61.apk)<br>
Version information: [Latest version](https://github.com/Imaginous/Cowboy_Untamed/releases/latest)

## Free accessories on your new bike
If you don't have a Cowbow bike yet... use this [refferal link](https://share.cowboy.com/r/michelv3) for €100 of free accessories on your new bike.

## Donate
If you like the app you're free to make a small donation.<br>You can do this securely via [PayPal](https://paypal.me/pools/c/8zcWXI7VnO).<br>
If you have a Dutch bank account you may also make your [donation via iDeal](https://betaalverzoek.rabobank.nl/betaalverzoek/?id=EkJA4Zm7Qpq1eDSKdddMeQ).

## Introduction

<img src="https://user-images.githubusercontent.com/68418842/117127423-59524780-ad9c-11eb-967d-f75f9e499da2.png" alt="Screenshot" width="250"/>

This app is created as a hobby project. I love electronics and programming and just could not resist if I could get more out of my Cowboy V1+ bike.

This is where I started finding out how the Cowboy bikes work. Which electronics they use and how the electronics communicate internally and with the outside world.
I posted on [Reddit](https://www.reddit.com/r/cowboybikes/comments/m6zrdx/disable_speed_limit/) and it got more attention then I had anticipated.

Special thanks go to Runereader for making his Bronco code open source.
This is my first Android app, pure hobby, so it is "as is".

## Installation
You must allow installation from unknown sources to install the Cowboy Untamed APK file.

- Goto `Settings` on your Android phone.
- Goto `Security`.
- Check the `Unknown Sources` option.

Now you should be able to download and install the APK file.

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

## The future
I think there is a quite solid base now for the future. Offcourse removing the speed limit was my main goal. Second I wanted to make shortcuts which I could use via *Tasker*.<br>I have discussed with other bikers and some of us would like to be able to set the support level. When you want to ride along with a non e-biker the support should be a lot less. The idea is to make speed dependant support. Let's say 0-10km/h you get the current support, 11-22km/h low to no support, 23->km/h regular untamed support. The levels can be set by the user. You can activate them via a long press shortcut.<br><br>These are ideas. I'm now ready to start exploring how to. I believe it can be done, but I want to do some serious testing with my own bike before I release it into the wild.

## FAQ

- Will there be an IOS version?<br>No, unfortunately I do not have (and have no intention to) an Apple developers account.<br>But you can do it manually, see: [IOS.md](https://github.com/Imaginous/Cowboy_Untamed/blob/main/IOS.md).
- Why should I enter 15% or 18% for the field weakening values?<br>These are merely my advise. The lower you keep the percentage the better it is for your battery range. At the moment I'm using 18% on my V1+ bike. It feels speedy enough, going faster makes my legs go round like a mad man. It's fun for a while, but not for a longer stretch. So 18% is my sweet spot. I assume on a V3 bike 15% is a more likely figure because of the lower gear ratio compared to the V1 and V2.
- Can the settings be undone?<br>Yes, if you have not tinkered with this app (or other apps like Bronco) you can write down your settings and re-apply them later. Using the defaults button can be tricky if Cowboy changes their default settings. Until now they didn't so you should be safe.
- I want to make a donation, how?<br>[Donate via PayPal](https://paypal.me/pools/c/8zcWXI7VnO)<br>If you have a Dutch bank account, [Donate via iDeal](https://betaalverzoek.rabobank.nl/betaalverzoek/?id=EkJA4Zm7Qpq1eDSKdddMeQ).
