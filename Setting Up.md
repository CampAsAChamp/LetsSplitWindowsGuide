# SETTING UP

### Table of Contents

- **Setting Up and Installing Software**
- [**Building** your keymap and keyboard firmware](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Building%20Firmware.md)
- [**Flashing** your Let's Split with your created firmware](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Flashing%20Firmware.md)

---

1) Install Bash Shell on Windows, follow [this guide](http://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/)

2) Download and install **AVRDudess**, [link here](http://blog.zakkemble.co.uk/avrdudess-a-gui-for-avrdude/)

3) Download and install **WinAVR or LIBUSB** to get the `LIBUSB0.DLL`
> * If you don’t then attempting to flash the pro micro won’t do anything     
> * I’m going to be using [WinAVR](http://winavr.sourceforge.net/index.html) for this, so download and install it

4) Go to install location of WinAVR and go to to the following path, using mine as an example 

**`C:\Program Files (x86)\WinAVR\utils\libusb\bin`**

![](http://i.imgur.com/0QiBvd0.png)

5) Copy the **4 `libusb0` files** from the WinAVR folder into the AVRDUDESS Program Files location and it should look like this now 

![](http://i.imgur.com/JPpaRmA.png)

6) **Clone with Git or Download the QMK Zip and unzip it** 

https://github.com/qmk/qmk_firmware 
> * For this guide I’m going to make it easy and just download the Zip 

![](http://i.imgur.com/v3sh3XQ.png)
      
7) **Extract the zip** so you have a folder named **QMK or qmk_firmware_master**
> * Place this in a nice easy location, that doesn’t require administrator access, like your documents folder or desktop

8) **Open a bash shell window** through the start menu (should be called bash.exe or Bash on Ubuntu on Windows)

9) **Change the directory to your QMK copy**, which you just unzipped.

![](http://i.imgur.com/z7NG8W0.png)

* Do this using the `cd` command (Hard drives are accessed in bash by typing `cd /mnt/<driveletter>`)

Example `cd /mnt/c/Users/Nick/Documents/qmk_firmware_master`

10) Run **`sudo util/install_dependencies.sh`**, This will run `apt-get upgrade`

11) Wait a while (5 minutes for me), and then you are good to go

### [Next Step(Building firmware)](https://github.com/CampAsAChamp/LetsSplitWindowsGuide/blob/master/Building%20Firmware.md)