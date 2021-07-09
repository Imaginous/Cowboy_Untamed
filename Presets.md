# Presets

A way to use Cowboy Untamed without storing any configuration persistantly in your bike.
This functionality can only be used on Android.

## Introduction

Some Cowboys out there are not comfortable with storing/altering their motor controller settings. For those Cowboys and those whom want to use an alternative setting once a while.
Presets can be a solution. The values set with a preset are lost when the bike is locked or the battery is removed.
Also it brings the posibility the lower the motor support to make you work harder and preserve some battery power.

The configuration is done through the main Cowboy Untamed app via menu *Quick Launch Presets*. You have to be connected to your bike, even for configuring the presets. Some values are internally specific per version of each Cowboy bike. Therfore I need to fetch them tot calculate the correct value.<br>
After configuration use the second app icon to start presets. Just long press the app icon to select a preset. Clicking the icon will activate the last used preset.

**Note:** do not use the *FLASH* button in the main app while a preset is active. This will store the preset settings in flash memory.

## Configuration
To configure the *Quick Launch Presets* connect to your bike and go to the corresponding menu in the main app.<br>
**Note**: empty fields are not send to the bike. The default values stored in the motor controller are used. So if you do not want to alter a certain value just leave it empty.

Explanation of the various values:
- **Launch Cowboy app when preset is activated**:
<br>When you toggle this switch to on, the original Cowboy app will be launched after the preset is activated.
- **Speed Mode #**: select the preset you want to alter. Note the names are just names, you can go fast with slow and vice versa.
<br>1 (Slow)- Use this to go slower then your normal preset.
<br>2 (Normal)- Use this as your default preset.
<br>3 (Fast)- Use this to go faster then your normal preset.
- **Field Weakening 0-25%:**
<br>*Empty* the speed limit is enforced and no field weakening is applied (default Cowboy setting). 
<br>0 only the speed limit is removed, no field weakening is applied. 
<br>1-25 the speed limit is removed. The value is the amount of field weakening applied. 
- **Peddle Max Torque:**
<br>It's an imaginary value. It calculates an offset to the default max torque sensor output voltage. 100% means the default torque sensor voltage. Decreasing this value will increase the maximum torque voltage value. This means that maximum throttle needs more torque input... hence you have to peddle harder.<br>This value is the easiest way to make the pedal resistance higher. You have to apply more force and therefore will save battery power.<br>The drawback is that going uphill will also be harder.
- **#. Maximum power 0-100%:**
<br>The motor controller allows for 8 preset points to set the maximum power output. In the description below the title you see the specific speed range for which the power level is used. This way you can still have all power available at low speeds but decrease the power output at higher speeds. Or any way you like.
<br>100% is standard full support, 0% means no motor support at all.
<br>I use this setting when cycling along non e-bikers. I still can get going easely but when at speed just drop the power output to get more resistance while peddling. I find it more comfortable to have some resistance.

After you set your values press **STORE PRESET**, this will not send anything to your bike. This only stores the settings in the app.
Disconnect from your bike on the *MAIN SCREEN*. Now long press *Cowboy Untamed Presets* icon and select the wanted preset. Clicking the icon will start the last preset.

**Note:** using presets will not alter any settings used with the *FLASH* method when a field is left empty. So if you set your field weakening to 18% with the *FLASH* method and you leave the field empty in the presets, 18% will be used. If you enter 0, the speed limit will be enforced without any field weakening. As soon as you lock the bike the preset is gone. So the next time you just unlock your bike the 18% field weakening will be applied again.

## My preferred Cowboy V1+ settings
The following screenshots show settings which give quite pleasant settings for me. Note it's all to preference.

<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/125077364-512ac700-e0c1-11eb-9a87-b3722a61099e.png" alt="Example Preset Slow" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/125077386-56881180-e0c1-11eb-8da6-c47a63a04d2a.png" alt="Example Preset Normal" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/125077399-5ab42f00-e0c1-11eb-9f2e-5df24054556e.png" alt="Example Preset Fast" width="250"/>
</p>

