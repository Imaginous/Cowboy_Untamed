# Cowboy Customization
In this document I will try to collect special customizations I made to my Cowboy bike. I also will try to supply information, photo's and files so you make the modifications yourself.

It won't be complete tutorials, you need to use your own skills and brains, but it will be doable.
Also note that I own a **Cowboy V1+**, not everything is the same on all bike models.

## Index
- [Battery charging 'hack'](https://github.com/Imaginous/Cowboy_Untamed/edit/main/Customization.md#battery-charging-hack)
- [New headlight design](https://github.com/Imaginous/Cowboy_Untamed/edit/main/Customization.md#new-headlight-design)

## Donate
If you like the instructions, you're welcome to make a [donation](https://github.com/Imaginous/Cowboy_Untamed/blob/main/README.md#donate). 

## Battery charging 'hack'

### Introduction
To keep the battery in the best shape it's commonly known to keep lithium-ion batteries between 20%-80% charge. This specially goes for phone batteries.
A bike battery is a bit different, it contains multiple series and parallel connected cells. Those cells should have the same state of charge and voltage.(theoratically).
In normal use the cells will be quite in balance, but over time cells will degrade differently and there will be a difference in capacity. This capacity mismatch results in cells or groups of cells in parallel draining faster. There the BMS (battery management system) comes in. It levels out each individual cell (or strand). This process is needed once and a while. It is always performed at the end of each charging cycle. So it means charging to 100%... but thats not optimal.

### The 'hack' / fix
This is not an *easy* fix, but more of a workaround. In my home I have a Zigbee home automation system. Therefore I can use this system to measure the current drawn by the bike's charger and can aproxemately *tell* how much has been charged. This is because of the fact the battery will be charged at a 'constant' current up to 80%. Then it will go down logarithmic. As soons as I see the power drop below 105 watt I found out that this is about 80%. Then I will stop charging.<br><br>
What do we need to accomplish this?
- A power measuring switchable poweroutlet (**Zigbee**/WiFi)<br>
I use a [Blitzwolf power plug](https://www.blitzwolfeurope.com/3840W-EU-WIFI-Smart-Socket-BlitzWolf-BW-SHP2-Wifi).
You can also buy plugs [pre-flashed with Tasmota firmware](https://mediarath.de/en/collections/tasmota-gerate).
- A Zigbee hub or interface when working with zigbee, other control software if you go the wifi route.<br>
I use a [CC2652 based Zigbee stick](https://slae.sh/projects/cc2652/) in combination with my own software. But you could use something like [Home Assistant](https://www.home-assistant.io/).<br>

If you use a WiFi module you can probably also use [Home Assistant](https://www.home-assistant.io/). For the Zigbee route there are also integrated hubs and devices like Philips HUE and Tahoma.

All you have to do now is to turn off the charger when the power starts dropping. *Note:* you have to take some measurements because the power values may be (will be) different in each charger/battery combination. How to do this is completely dependend on the system you use.<br><br>
This solution is really for tweakers. So this is not a step by step tutorial, but just a guideline how to achieve this.<br>
**Important:** as stated earlier, you still need to balance the cells once and a while. Therefore I let my battery charge to 100% every 5th charging cycle.<br><br>

### General battery advice
This is just how I handle my battery over the last 1.5 years.
- Keep the charge between 20%-80%, but fully charge about every 5th charging cycle to balance the cells.
- Always leave the battery in the bike. This will keep the internal battery (for GPS and data communications) charged. Leaving this battery discharged for a longer period of time is not good for the battery.
- Store the bike in a warm and dry place (8-30 degrees celcius).
- Don't charge the battery when it's very cold or very warm. Bring it to room (or shed) temperature first.<br>Don't charge it directly after cycling, it has to cool down.
- When not using the bike for a longer period charge it to 80%.<br>
Turn off *Auto Unlock*.<br>
Don't let it go below 20%. So recharge the battery every 1 to 1.5 months up to 80%.

## New headlight design
About half a year ago I created a new lens/lamp cover for my Cowboy, it increased the light quite a bit. But now, when darker days are joining near, it's still not effective enough to my likings. So I developed *V2*.<br>
*2021-11-09*: The headlight mount on the Cowboy is tilted upwards by 10 degrees (not down for some reason). This made the V2 light shine up too much. Therefore I made V2b and V2c, this is angled down at 20 degrees. Since the used lenses are 20 degrees this technically means the upper part of the light bundle goes straight ahead now. The lower part is now angled at 10 degrees down. First indoor tests look way more promissing.<br><br>
The V2b and V2c are two flavours. Because the lenses are put in at an angle, Pythagoras dictates that the total height will be greater. Therfore it didn't fit in the original height available. I came to two solutions:
1. V2b - Make the front thicker and add an extra ring to block the light.
2. V2c - Place the headlight a bit deeper, but it won't snap into place anymore. Therefore I used double sided foam tape to fixate it.

**Note:** I know it's not as beautifull as the original cover, but I personally like this better then adding a seperate light.

### The materials used
- [7 lenzes from Ali Express](https://a.aliexpress.com/_uIxFhM)
- Transparent PET & white ABS 3D print filament
- *V2b* uses carbon fiber PLA filament (for a black bike)
- *V2c* method requires double sided foam tape.

### The 3D print files
- [3D print files V2](https://github.com/Imaginous/Cowboy_Untamed/files/7446418/Printing.zip)
- [3D print files V2b](https://github.com/Imaginous/Cowboy_Untamed/files/7507790/Printing_V2b.zip)
- [3D print files V2c](https://github.com/Imaginous/Cowboy_Untamed/files/7507804/Printing_V2c.zip)

### Basic instructions
You have to print the cover part with a multi material 3D printer to fuse the ABS and PET parts together. I use a variable layer height of 0.2mm for the first layer, then the other layers on 0.1mm. I use a Prusa 3D printer MII-Multi material V1.

Print the *bike reflector lens* (note: V2 only) with white ABS and a few pieces of doublesided foam tape underneath to stick it to the PCB later.

After printing I strengthen the clips by adding some super glue onto it. I use super glue which comes with a brush.
You can push in the lenses, if you want you can ad a very small drop of super glue on the left and right side of the lens.

**NOTE: Removing the headlight can be done destructive and non destructive. I used the destructive way.**
To remove the headlight the proper way you need to remove the entire front fork. As soon as you have taken it out you can push out two white clips. By doing so the entire headlight will pop out.

**The destruvtive way** is way easier, but you will break the clips of the original cover. This might be a problem if you want to put the bike back in it's original state. You can always buy a new headlight at Cowboy.
The trick is to put doublesided tape on the headlight (clean it first). Then add a large flat piece of metal (or wood) and pull straight out... the clips will break and you have the front light cover stuck to your piece of metal. Try to get the rest of the clips out so they won't fall into your steering tube. Now push the upper part into the bike and lift the lower part out. Slide it a bit down and pinch the two upper clips with your fingers. You can now pull the light slightly towards you. Not very far, because the cable is rather short.

Now stick the reflector part to the PCB (note the notches - V2 only). Now clip on your new cover with the lenzes in place (if you don't want to glue them stick them in place with a bit of tape on the front side, the lenzes will be snugg after it's clipped in place. you can then remove the tape).

**Test the light** and then place the unit back into the bike, first make sure the bottom bit is in as far as possible, then slowly push in the top part.

# The photo's V2b
<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/141002661-e596e824-66b3-4650-a7ce-db5043c993af.JPG" width="295"/>
<img src="https://user-images.githubusercontent.com/68418842/141002717-a6cb32f5-0bed-4159-b4fe-6264a1188b1f.JPG" width="295"/>
<img src="https://user-images.githubusercontent.com/68418842/141002727-adcbabee-48bb-4c51-9c71-e6ac6882b728.JPG" width="295"/>
</p>

# The photo's V2c
<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/141003031-eaa922e8-9a3f-4688-ac1a-cc6aebefad48.JPG" width="295"/>
<img src="https://user-images.githubusercontent.com/68418842/141003088-c3ecaa6c-0320-4d2e-835b-e691546a660e.JPG" width="295"/>
</p>

# The photo's original V2
<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/139531589-33d30365-ba35-4ca8-8e12-89ec61f20c40.JPG" height="250"/>
<img src="https://user-images.githubusercontent.com/68418842/139531592-6cea4fdf-b9b1-4d6f-a2c4-5902ed4eab53.JPG" height="250"/>
<img src="https://user-images.githubusercontent.com/68418842/139531595-0d93a763-5a3d-4340-b6f0-5ac2f5a5e162.JPG" width="295"/>
<img src="https://user-images.githubusercontent.com/68418842/139531601-15901260-c18a-434c-8b3a-62bb08eba48e.JPG" width="295"/>
<img src="https://user-images.githubusercontent.com/68418842/139531603-1bf23dd7-93ad-410d-969a-04e1500ab2cc.JPG" width="295"/>
</p>

