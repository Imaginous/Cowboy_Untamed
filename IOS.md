# IOS Users

You can use an Android phone to make the "hacks" or do some of them by hand using the [nRF Connect](https://apps.apple.com/nl/app/nrf-connect-bluetooth-app/id1054362403 "nRF Connect") app or the [BLE Scanner](https://apps.apple.com/nl/app/ble-scanner-4-0/id1221763603 "BLE Scanner") app from the Apple Store.

## Donate
If you like the instructions, you're welcome to make a [donation](https://github.com/Imaginous/Cowboy_Untamed/blob/main/README.md#donate). 

## Usage
Disable speedlimit Cowboy C1+, C2 and C3.
It's completely at your own risk, your bike will be "illegal" in most (European) countries. However the police cannot see it in the app.

**Unlock your bike with the Cowboy app.**
**Kill the Cowboy app and make sure it's not running in the backround.**

For more information on the nRF Connect app go to [here](https://devzone.nordicsemi.com/f/nordic-q-a/22523/writing-hex-values-to-characteristics-using-nrf-connect "here").

So use the nRF Connect app. It seems you have to connect to the Cowboy and then disable “Parse known characteristics". Now you can select "BYTE ARRAY" when sending. I assume this will solve the problem of the values not written correctly on some devices.
- Connect to your Cowboy and make sure it's connected and bonded.
- Go to Nordic UART Service Send values to RX Characteristic.
On some devices it might be shown as **CUSTOM SERVICE** address: `6E400001-B5A3-F393-E0A9-E50E24DCCA9E`.
- Select the sub UUID: `6E400002-B5A3-F393-E0A9-E50E24DCCA9E` and select *write* or the *W* button.
- Select *Byte Array* and send the wanted codes from the list below.

##### Disable / enable speed limit:
- Disable speed limit: `0110000b000102000166eb`
<br>or<br>
Enable speed limit (default): `0110000b000102000226ea`

##### Set field weakening (needed to go faster then 30km/h):
- Field weakening 18% (Recommended value for C1+, C2): `0110008100010202e17969`
<br>or<br>
Field weakening 15% (Recommended value for C3): `011000810001020266390b`
<br>or<br>
Field weakening 10% (Alternative value): `01100081000102019a39ba`
<br>or<br>
Field weakening 20% (Alternative value): `011000810001020333f8a4`
<br>or<br>
Field weakening 25% (**NOT RECOMMENDED** - Absolute maximum value): `011000810001020400ba81`
<br>or<br>
Field weakening 0% (default): `011000810001020000b841`

##### Resolve motor judder at start up:
- Hall Interpolation Transitions 8: `011000800001020008B856`
<br>or<br>
Hall Interpolation Transitions 15: `01100080000102000ff994`
<br>or<br>
Hall Interpolation Transitions 1 (default): `0110008000010200017850`

##### To make the changes "persistant" after lock or battery removal:
- Store in flash: `011001ff0001027fffc2ef`<br>followed by<br>
Close flash: `011001ff0001020000a29f`
- **Note:** Not needed for testing as long as you don't lock the bike.

If you have followed the steps above the settings should be made and you can start using the regular Cowboy app again.

##### Enable / Disable *Auto Unlock* (on a C1+):
- Enable *Auto Unlock*: `0A100014000102000117B4`
<br>or<br>
Disable *Auto Unlock*: `0A1000140001020000D674`
- **Note:** You don't need to store this value to flash. It's immediately active.


##### Reset PCB (fix headlight bug on C1+):
- Reset: `0A1000F2000102000101B2`
- **Note:** The bike will reset and will show a 2 led running light on the main tube to indeicate the PCB reset.<br>You won't lose any settings it's just a restart of the PCB.

## Why isn't there an IOS app?
Many people ask me why there is no IOS app?
- First of all I'm not an IOS developer. To become an IOS developer Apple charges €200,- per year.
- Furthermore you need Apple devices to develop on and test with.
- Also "side loading", putting an app on your phone outside the *Apple Store* is almost impossible for non developers. So you need a developer account yourself at the cost of €200,- per year.
- Another developer contacted me willing to make an IOS version. However after some research it seems to be difficult to get the app approved for the *Apple Store* due to the *hack* nature of it. Also the developer of the *Moofer app* (for van Moof bikes) pointed out that he had a lot of problems getting his app in the *Apple Store*. It's finally allowed because it basicly only changes the country in which the bike is used.
- All in all for me it's just not worth it to go through all this trouble and since I don't own any recent Apple devices I don't feel any personal need for it.
- You can do the manual *hack* with the provided information below, which I gathered during my research.

I'm sorry cowboys and girls, but Android is just more open minded and *hacker* friendly ;)


