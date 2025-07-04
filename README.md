# Gamesir (T4) Nova Lite Linux Guide

**DISCLAIMER: WIP? No, I think I'm done.**

This guide will help you deal with:

- lack of manual out of the box
- pairing issues when gamepad can't reconnect
- inability to switch gamepad mode when connected via reciever
- non-working vibration (rumble) on linux when connected via bluetooth
- missing xbox mode (xinput)

To solve these problems, the following steps can be done:

- Change gamepad firmware version to 4200 or 6300 (which is not avaliable by default in the official **gamesir world app**)
- Install USB reciever firmware (optional, for 6300 gamepad firmware, but will not work with 4200 gamepad firmware)
- Install and configure [xpadneo](https://github.com/atar-axis/xpadneo) driver for a PC with Linux-based operating system on it.

## 0. Gamepad Functions Manual

[Link to official manual](https://cdn.shopify.com/s/files/1/2241/8433/files/Manual-GameSir_Nova_Lite_EN.pdf?v=1743156237)

**DISCLAIMER**: this PDF file is heavy

<details> <summary> 

### 0.1 (Official) Device layout (*click to show/hide section*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/bdf238e4-da55-4e89-ad1c-411c8057f9db" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/7d091089-3069-41c6-82cd-c98e1de190db" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/71148763-3677-4dc8-a48d-592090af3ca1" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/5a5d2da8-d133-4237-b0ad-a2297906e16d" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 

### 0.2 (Official) Basic functions (*click to show/hide section*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/15016cb6-4045-4126-af35-6811b298e1f6" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/423a32c8-80d0-49fe-820a-36fc64647c8a" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/c5b1d93c-c6e1-40e5-a69b-679830210f0e" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 
  
### 0.3 Reactivate pairing (*click to show/hide section*) </summary>
 
If reconnection is failing or you want to use your gamepad with another device, then you need to enable ***pairing mode***.

To do this, hold the ```HOME``` and ```SCREENSHOT``` buttons for 3 seconds (no more, otherwise the controller will turn off):

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/542149f6-fb97-46ce-b17c-a74a179882e4" alt="drawing" width=50%/> </p>

Then you can connect to your gamepad via bluetooth or reciever again.

This works with every [connection method](#04-official-connections-tutorial-click-to-showhide-section-).

</details>

<details> <summary> 
  
### 0.4 (Official) Connections tutorial (*click to show/hide section*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/d7d2f1a1-0b8a-46bc-8a76-d6f9d052efcd" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/8c366ea5-b933-4855-8052-cb92d3ee64d6" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/25f33e83-5332-47ef-ab3b-c6f0cbe72cc6" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/50afb1b4-7b1d-4eaa-bbb1-09d8bba9202c" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/d8ff7099-dde8-40ee-8335-31d0dff7a7e8" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 
  
### 0.5 (Official) Advanced tutorial (*click to show/hide section*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/ab65eb2f-ce84-4418-85a7-79661505e80c" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/299f106f-5a30-4607-8acb-d4d117d49d01" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/bd1442e7-c3e1-46b5-8dd5-ef9a84d55835" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/dc62f13f-ce05-440c-9027-03cf7f6a6546" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/4d713cda-a437-46a2-9297-ed4f25b712dd" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 

### 0.6 Fast reconnect (*click to show/hide section*) </summary>

To quickly turn on the gamepad and automatically connect to the last remembered device, hold the ```HOME``` button for one second.

</details>

<details> <summary> 

### 0.7 Turn off (*click to show/hide section*) </summary>

To turn off the gamepad, hold down the ```HOME``` button for more than 4 seconds until the light around the button turns off.

</details>

</details>

## 1. Upgrading/downgrading firmware

Before doing any serious actions with your device (for which I am not responsible, by the way, **you do all these actions at your own risk**), I advise you:

1. Download the official GameSir World App application to your smartphone (in the Play Market it may be called simply GameSir)
2. Connect your gamepad to your smartphone (using the A + HOME buttons on the gamepad. Note: if the gamepad is not in the list of Bluetooth devices, see the [0.3 Reactivate pairing](#03-reactivate-pairing-click-to-showhide-section-) section)
3. Add the gamepad to the GameSir application and look at the firmware version, perhaps you already have version 6300, if not, I advise you to install version 4200 which is more stable, than latest 6900 or 5700.

<details> <summary> 

### 1.1. Firmware 4200 </summary>

### 1.1.1 Gamepad Firmware 

<img src="https://github.com/user-attachments/assets/62f34d59-4879-4d3f-a744-d67a08b96eea" alt="drawing" width=30%>
<img src="https://github.com/user-attachments/assets/3016f78d-e699-401c-a601-ad28da78566a" alt="drawing" width=30%/> </p>

On the gamepad, press the ```A```+```HOME``` buttons until the HOME button starts blinking yellow. If it blinks slowly, the gamepad will not appear in the list of Bluetooth devices. In this case, see [0.3 Reactivate pairing](#03-reactivate-pairing-click-to-showhide-section-) section.

<img src="https://github.com/user-attachments/assets/d7c39f12-d59c-4b0b-b6a2-88ec399d31f9" alt="drawing" width=30%/>
<img src="https://github.com/user-attachments/assets/8a20775b-69f0-4397-821c-11522b544c83" alt="drawing" width=30%/>
<img src="https://github.com/user-attachments/assets/88cae5bc-7a3b-4298-8ca7-57436a5a80c7" alt="drawing" width=30%/> </p>

Now open Gamesir app and add your gamepad in the Devices section. If you already have the device added, like in the following screenshot, you can click on the big icon of your gamepad right away.

<img src="https://github.com/user-attachments/assets/4be22856-9515-46af-99a1-34e3bcde78c2" alt="drawing" width=30%/>
<img src="https://github.com/user-attachments/assets/dd88c593-cd65-4293-af35-c6817a090c74" alt="drawing" width=30%/>
<img src="https://github.com/user-attachments/assets/ba0220d5-5374-4e19-8103-7aa165357ce2" alt="drawing" width=30%/> </p>

After pressing the "Continue Upgrade" button, the gamepad will disappear from the list of Bluetooth devices, and the backlight around the HOME button will start to blink slowly. At this point, you can cancel everything, and to connect the gamepad to smartphone again, see [0.3 Reactivate pairing](#03-reactivate-pairing-click-to-showhide-section-) section.

<img src="https://github.com/user-attachments/assets/9c2ac8b7-26e1-4b18-ac3a-8631217f222a" alt="drawing" width=30%/> </p>

As you can see in screenshot below, I already have firmware version 6300. Perhaps you will already have it after purchasing the device. Then, you probably can end read this guide.

If it isn't, let's move on.

<img src="https://github.com/user-attachments/assets/f4ea8099-a724-4ee5-8636-67f36915c513" alt="drawing" width=30%/> 
<img src="https://github.com/user-attachments/assets/e503317f-b8c8-47dd-b657-9cdd4eb4744d" alt="drawing" width=30%/>
<img src="https://github.com/user-attachments/assets/6d365742-7bb6-4fa5-b403-cad26e63b5a5" alt="drawing" width=30%/> </p>

**ATTENTION**: next you will need to agree to install the firmware. Make sure that your smartphone and gamepad have enough battery power, and your internet connection is stable.
If the update fails to download and the controller indicator is still flashing and not off, you can still cancel the process and try connecting to a more stable internet connection or using a VPN.

After downloading the firmware, the gamepad will go into **"firmware update mode"**: the backlight around the HOME button will go out, the device will disappear from the list of connected Bluetooth devices, ***but it's actually connected***.
I strongly recommend that you do not interrupt the process at this stage, do not minimize the application, do not turn off the smartphone screen, and do not move the two devices far from each other.

**ATTENTION**: If for some reason the firmware installation is not completed successfully, your gamepad will still be in **"firmware update mode"**, it will still be connected to your smartphone (despite the fact that the device will not be in the list of connected Bluetooth devices), and you will most likely be able to repeat the firmware installation process inside Gamesir app (firmware upgrade button will be avaliable).

<img src="https://github.com/user-attachments/assets/eaad63b5-c008-4d28-90d2-c47b758c5b69" alt="drawing" width=30%/> 

### 1.1.2 Reciever Firmware

Not required when working well with the 4200 gamepad firmware.

</details>

<details> <summary> 

### 1.2. Firmware 6300 </summary>

You can find the official manual and firmware/software files [here](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html). For some reason, this guide is only available in Chinese.

### 1.2.1 Gamepad firmware

You can install this version of firmware in two ways: 
1. via a smartphone and Gamesir World App
2. via a Windows PC and special firmware update software.

<details> <summary> 

### 1.2.1.1. Via Gamesir World App </summary> 

The process is the same as in [Firmware 4200](#11-firmware-4200-) section, but in order for firmware 6300 to appear among the available ones in the list, you need to change the language of your device to Chinese (simplified).

Here is the proof:

<img src="https://github.com/user-attachments/assets/09c0b28b-6640-4bab-bdfc-52381b613d56" alt="drawing" width=30%/> 

</details>

<details> <summary>

### 1.2.1.2. Via Firmware Update Software for Windows </summary> 

Windows PC is required for this. Virtual machine is not acceptable. You can try use some WinPE iso's...

Open [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

From there get first two zip archives

![Снимок экрана_20250704_002412](https://github.com/user-attachments/assets/abd93fe5-2480-4702-8d95-cf5a7cfd6878)

Extract files from archives into one folder. Then do the same as says on screenshots of [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

<details>
<summary>
  
#### Click to show step-by-step instruction in screenshots </summary>

<img src="https://github.com/user-attachments/assets/fd5b1027-f8fa-4f39-b976-05f2731582bb" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/98542ca3-30ad-4004-818b-d11720e9ff92" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/5078cab0-bb57-494c-bd00-fecbab94908b" alt="drawing" width=70%/> </p>

The next step requires a wired connection between the gamepad and the PC.

<img src="https://github.com/user-attachments/assets/cb4be9c6-d64a-44a3-b7f9-3eb7c898d022" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/18aa435c-e2a2-41ac-a6bc-5bc3379c0828" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/2831a110-4ce5-4cae-96f7-142a1ace46c8" alt="drawing" width=70%/> </p>

</details> 

</details>

<details> 
<summary> 

### 1.2. USB reciever firmware (optional) </summary>

**ATTENTION**: as far as I know, after this you can't expect from your gamepad with 4200 firmware work with updated reciver. And you can't go back after this.

Windows PC is required for this. Virtual machine is not acceptable. You can try use some WinPE iso's...

Open [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

From there get first and third archives

![Снимок экрана_20250704_185012](https://github.com/user-attachments/assets/439dba72-907f-4400-9e0f-d61ae1129800)

Extract files from archives into one folder. Then do the same as says on screenshots of [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

<details>
<summary>
  
#### Click to show step-by-step instruction in screenshots </summary>

<img src="https://github.com/user-attachments/assets/fe123609-cf7e-4dd0-9bcf-b15343351706" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/c6e35375-d952-4285-b2a0-3b5d94da7127" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/124ce226-a81f-443b-8261-47d195f3afdf" alt="drawing" width=70%/> </p>

Now, connect the receiver to the computer, while holding down the button on it. After the indicator light stops glowing, continue.

<img src="https://github.com/user-attachments/assets/799b1204-1d14-4f39-8356-5625b7fe9710" alt="drawing" width=70%/> </p>
<img src="https://github.com/user-attachments/assets/3ab13c61-60d1-4767-88cb-8027fab40b30" alt="drawing" width=70%/> </p>

</details> 

</details>

</details>

## 2. Install xpadneo driver on Linux-based distro

[Xpadneo driver](https://github.com/atar-axis/xpadneo) is designed to work with the Bluetooth protocol, for us it will do two things:

1. Detect xinput mode (```B```+```HOME```) as ```XBOX 360 Controller``` (may be useful for some old games that works with this gamepad only)
2. Allow vibration (rumble) to work in xinput mode (```B```+```HOME```)

<details> 
<summary> 

### 2.1. Installation </summary>

Check [this section](https://github.com/atar-axis/xpadneo?tab=readme-ov-file#prerequisites) and do [these steps](https://github.com/atar-axis/xpadneo#installation) from original instruction of xpadneo driver.

</details> 

<details> 
<summary> 
  
### 2.2. Post-installation configuring </summary>

Create file ``` 99-gamesir-nova-lite-gamepad.rules ``` in ``` /etc/udev/rules.d/ ``` 

with:

```
KERNEL=="hidraw*" ATTRS{name}=="Xbox Wireless Controller" GROUP="input", MODE="0660", TAG+="uaccess"
SUBSYSTEMS=="input", ATTRS{name}=="Xbox Wireless Controller", GROUP="input", MODE="0660", TAG+="uaccess"
KERNEL=="hidraw*" ATTRS{name}=="2.4G XBOX 360 For Windows" GROUP="input", MODE="0660", TAG+="uaccess"
SUBSYSTEMS=="input", ATTRS{name}=="2.4G XBOX 360 For Windows", GROUP="input", MODE="0660", TAG+="uaccess"
KERNEL=="hidraw*" ATTRS{name}=="Zikway Pro Controller" GROUP="input", MODE="0660", TAG+="uaccess"
SUBSYSTEMS=="input", ATTRS{name}=="Zikway Pro Controller", GROUP="input", MODE="0660", TAG+="uaccess"
KERNEL=="hidraw*" ATTRS{name}=="Zikway HID gamepad" GROUP="input", MODE="0660", TAG+="uaccess"
SUBSYSTEMS=="input", ATTRS{name}=="Zikway HID gamepad", GROUP="input", MODE="0660", TAG+="uaccess"
```

<details> 
<summary> 

#### Click to show how to do this </summary>

> Just run in terminal this command to open **nano** editor
> 
> ```console
> sudo nano /etc/udev/rules.d/99-gamesir-nova-lite-gamepad.rules 
> ```
> 
> copy code above
> 
> And paste it in **nano** with ```ctrl``` + ```shift``` + ```v``` shortcut
> 
> Then ```ctrl``` + ```s``` to save
> 
> Then close **nano** with ```ctrl``` + ```c```

</details>

### 2.2.1 Fix rumble

Create (or edit, if exists) file ```99-xpadneo-options.conf``` in ```/etc/modprobe.d/```

in the end of this file add line with:

```
options hid_xpadneo quirks=44:24:C4:xx:xx:xx+6
```

<details> 
<summary>

#### Click to show how to do this </summary>

> Just run in terminal this command to open **nano** editor
> 
> ```console
> sudo nano `/etc/modprobe.d/99-xpadneo-options.conf
> ```
> 
> In **nano** press the ```Down``` button on keyboard until you reach the end of the file, also after that you can press ```Enter``` button on keyboard several times to create new blank lines
>
> copy code above
> 
> And paste it in **nano** with ```ctrl``` + ```shift``` + ```v``` shortcut
> 
> Then ```ctrl``` + ```s``` to save
> 
> Then close **nano** with ```ctrl``` + ```c```

</details>

Where ***4:24:C4:xx:xx:xx*** is MAC adress of ***your*** gamepad

You can find it in the list of bluetooth devices, in the system applet or **blueman**

![Снимок экрана_20250704_144425](https://github.com/user-attachments/assets/6e29d062-b9dc-4da6-b204-b0146134ac68)

After the address, be sure to add a prefix (+6), without spaces. You can find out more details about this [here](https://github.com/atar-axis/xpadneo#gamesir-t4-nova-lite-family)

</details>
