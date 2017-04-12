# BUILDING HEX

### Table of Contents

- [**Setting Up** and Installing Software](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Setting%20Up.md)
- **Building** your keymap and keyboard firmware**
- [**Flashing your Let's Split with your created firmware](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Flashing%20Firmware.md)

## For the default keymap, with no customization

1) Change the directory to your Lets_Split folder 

![](http://i.imgur.com/C4omjSV.png)

* Do this using the **`cd`** command 

Hard drives are accessed from `cd /mnt/<driveletter>`

Example `cd /mnt/c/Users/Nick/Documents/qmk_firmware_master/keyboards/lets_split`

2) Type **`make`** and it will build all of the hex’s that are available by default (Serial and i2c, for both Rev 1 & Rev 2) 

![](http://i.imgur.com/1Kz4znI.png)

3) Your hex file and a folder will be generated for you at the following location **`qmk_firmware_master/.build`**	 	

> * This folder will be generated and your appropriate hex files will be inside, all you need is your .hex file, so copy that somewhere safe, or you can just drag it in the let’s split folder in QMK 

![](http://i.imgur.com/DaOXSil.png)

## For customization

1) **Change the directory to your Lets_Split folder**

![](http://i.imgur.com/C4omjSV.png)

* Do this using the **`cd`** command 

Hard drives are accessed from `cd /mnt/<driveletter>`

Example `cd /mnt/c/Users/Nick/Documents/qmk_firmware_master/keyboards/lets_split`

2) Customize and configure your files in the Rev 2 folder (keymap.c for layout, but check QMK wiki on GitHub for more advanced)

> * Only if using Rev 2 PCB, **if you are using Rev 1 just do everything in Rev 1 folder**, and type **`make rev1`**

* For me, I had to reverse the right side, because it was flipped, read the instructions for that above, at the end of the _zsh's guide, he goes over how to fix this. I’m not going to go into customization in this guide, so just check the QMK Wiki

3) Type **`make rev2`**

4) Your hex file and a folder will be generated for you at the following location **`qmk_firmware_master/.build`**

> * This folder will be generated and your appropriate hex files will be inside, all you need is your .hex file, so copy that somewhere safe, or you can just drag it in the let’s split folder in QMK 

![](http://i.imgur.com/DaOXSil.png)

### [Next Step(Flashing firmware)](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Flashing%20Firmware.md)