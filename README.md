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

The Test button will only send the values to the bike. As long as you are connected to the bike and it's unlocked you can test drive with these values. When the bike is locked or the battery is removed the values are reset.

Press Flash if you want to store the settings permanently. These are kept in the flash memory of the motor controller and you can use them with the original Cowboy app.

Pressing Defaults will set the dialog to their default values as used by Cowboy. You need to press the Test followed by the Flash button to store them in the motor controller.

