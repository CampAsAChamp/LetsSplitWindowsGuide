# BUILDING HEX

### Table of Contents

- [**Setting Up** and Installing Software](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Setting%20Up.md)
- **Building your keymap and keyboard firmware**
- [**Flashing** your Let's Split with your created firmware](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Flashing%20Firmware.md)

---

## For the default keymap, with no customization

1) Change the directory to your QMK folder 

![](https://i.imgur.com/Yolz2bJ.png)

* Do this using the **`cd`** command 

Hard drives are accessed from `cd /mnt/<driveletter>`

Example `cd /mnt/c/Users/Nick/Documents/qmk_firmware_master/`

2) Type **`make lets_split-rev2`** and it will build all of the hex’s that are available by default (Serial and i2c, for both Rev 1 & Rev 2) 

![](https://i.imgur.com/kzpCKaH.png)

3) Your hex files will be generated for you in the same folder, **`qmk_firmware_master/`**	 	

> * All you need is your lets_split_rev2_default.hex file 

![](https://i.imgur.com/uR1Q7F0.png)

## For customization (Skip if you wanted just the default layout, steps for that are above)

1) Customize and configure your files in the Rev 2 folder (keymap.c for layout, but check [QMK docs](https://docs.qmk.fm) on GitHub for more advanced)

> * Only if using Rev 2 PCB, **if you are using Rev 1**, type **`make lets_split-rev1-<keymap>`**

* For me, I had to reverse the right side, because it was flipped, read the instructions for that above, at the end of the _zsh's guide, he goes over how to fix this. I’m not going to go into customization in this guide, so just check the [QMK Docs](https://docs.qmk.fm)

3) Type **`make lets_split-rev2-<keymap>`** and replace `<keymap>` with your keymap, for example: `make lets_split-rev2-nick`

![](https://i.imgur.com/6wbxeEX.png)

4) Your hex file will be generated for you in the root folder, **`qmk_firmware_master/`**

> * All you need is your .hex file, so copy that somewhere safe, or you can just drag it in the let’s split folder in QMK 

![](https://i.imgur.com/jqVpwl9.png)

### [Next Step(Flashing firmware)](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Flashing%20Firmware.md)
