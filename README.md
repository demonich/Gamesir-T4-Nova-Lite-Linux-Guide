# Gamesir (T4) Nova Lite Linux Guide

**DISCLAIMER: WIP. The guide is not done yet**

This guide will help you deal with:
- pairing issues when gamepad can't reconnect
- inability to switch gamepad mode when connected via reciever
- non-working rumble (vibration) on linux when connected via bluetooth
- missing xbox mode (xinput)

To solve these problems, the following steps can be done:
- Change gamepad firmware version to 4200 or 6300 (which is not avaliable by default in the official **gamesir world app**)
- Install USB reciever firmware (optional, for 6300 gamepad firmware, but will not work with 4200 gamepad firmware)
- Install and configure [xpadneo](https://github.com/atar-axis/xpadneo) driver for a PC on Linux

## 0. Gamepad Functions Manual

[Link to official manual](https://cdn.shopify.com/s/files/1/2241/8433/files/Manual-GameSir_Nova_Lite_EN.pdf?v=1743156237)

**DISCLAIMER**: this PDF file is heavy

<details> <summary> 

### 0.1 Device layout (*click to show/hide images*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/bdf238e4-da55-4e89-ad1c-411c8057f9db" alt="drawing" width=70%/> </p>

<img src="https://github.com/user-attachments/assets/7d091089-3069-41c6-82cd-c98e1de190db" alt="drawing" width=70%/> </p>

<img src="https://github.com/user-attachments/assets/71148763-3677-4dc8-a48d-592090af3ca1" alt="drawing" width=70%/> </p>

<img src="https://github.com/user-attachments/assets/5a5d2da8-d133-4237-b0ad-a2297906e16d" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 

### 0.2 Basic functions (*click to show/hide images*) </summary>

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/15016cb6-4045-4126-af35-6811b298e1f6" alt="drawing" width=70%/> </p>

<img src="https://github.com/user-attachments/assets/423a32c8-80d0-49fe-820a-36fc64647c8a" alt="drawing" width=70%/> </p>

<img src="https://github.com/user-attachments/assets/c5b1d93c-c6e1-40e5-a69b-679830210f0e" alt="drawing" width=70%/> </p>

</details>

<details> <summary> 
  
### 0.3 Reactivate pairing (*click to show/hide images*) </summary>
  
To activate the pairing status, you need to hold down the HOME and SCREENSHOT buttons for 3 seconds:

*click on images to enlarge*

<img src="https://github.com/user-attachments/assets/542149f6-fb97-46ce-b17c-a74a179882e4" alt="drawing" width=50%/> </p>

Then you can connect to your gamepad via bluetooth or reciever again if reconnection is failed or you want to use gamepad with another device

</details>

## 1. Install firmware

You can find the official manual and firmware/software files [here](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html). For some reason, this guide is only available in Chinese.

### 1.1. Gamepad firmware

You can change firmware of this gamepad in two ways: via a smartphone or via a Windows PC.

### 1.1.1. By Gamesir World App

**DISCLAIMER**: I personally did these steps on my Android device and can't provide instructions for iOS users (it should be almost the same I think)

Get latest version of Gamesir App from [official website](https://gamesir.com/pages/software-detail)

![Снимок экрана_20250703_233114](https://github.com/user-attachments/assets/550d5377-9ae4-44f8-add7-cff7f173016f)

After installing the application, connect the gamepad to your smartphone. To do this, on gamepad press A + HOME buttons. The HOME button will start flashing yellow around. In the smartphone settings, go to Bluetooth, go to something like "search for devices" where in the list there will be "gamesir nova light"

If the device name is not in the list, it means that the gamepad cannot reconnect to the device that it remembered last. To put the gamepad into pairing mode, press HOME button and *the button below it* for 3 seconds. The backlight will start flashing faster, and you will be able to connect to the gamepad.

Inside the gamesir app, add your gamepad: in the device tab, in the upper right corner, click on the gamepad with plus icon, In the appeared list of devices find "gamesir nova lite"

Now, change your device settings to chinese. Yep, without this step, the application will not display the firmware version we are interested in.

**DISCLAIMER**: Actually, you can install firmware 4200, which is works well, other firmwares after this version work poorly (except 6300)

After that, open the gamesir application again and follow the steps shown in the screenshots:

<details>
<summary>
  
#### Click here
</summary>

<img src="https://github.com/user-attachments/assets/c8d4370d-0cd5-44b4-9fc7-74e0688e2876" alt="drawing" width="250"/> </p>

<img src="https://github.com/user-attachments/assets/8b01f2cd-d186-447c-8692-f1da2caae281" alt="drawing" width="250"/> </p>

<img src="https://github.com/user-attachments/assets/63746b55-aaff-4c01-882d-8eca2fcac586" alt="drawing" width="250"/> </p>

<img src="https://github.com/user-attachments/assets/09c0b28b-6640-4bab-bdfc-52381b613d56" alt="drawing" width="250"/> </p>

<img src="https://github.com/user-attachments/assets/f86c6936-9321-4d7e-870d-46f5ebda2db5" alt="drawing" width="250"/> </p>

</details> 

After this, do not forget to return the language settings to their original state.

### 1.1.2. By Windows Software

You should do this steps on Windows (you can try use some winPE iso's..., virtual machine however is not acceptable for this)

Open [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

From there get first two zip archives

![Снимок экрана_20250704_002412](https://github.com/user-attachments/assets/abd93fe5-2480-4702-8d95-cf5a7cfd6878)

Extract files from archives into one folder. Then do the same as says on screenshots of [official guide](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html)

<details>
<summary>
  
#### Or look here
</summary>

<img src="https://github.com/user-attachments/assets/fd5b1027-f8fa-4f39-b976-05f2731582bb"/> </p>

<img src="https://github.com/user-attachments/assets/98542ca3-30ad-4004-818b-d11720e9ff92" alt="drawing" width="600"/> </p>

<img src="https://github.com/user-attachments/assets/5078cab0-bb57-494c-bd00-fecbab94908b"/> </p>

<img src="https://github.com/user-attachments/assets/cb4be9c6-d64a-44a3-b7f9-3eb7c898d022" alt="drawing" width="700"/> </p>

<img src="https://github.com/user-attachments/assets/18aa435c-e2a2-41ac-a6bc-5bc3379c0828" alt="drawing" width="600"/> </p>

<img src="https://github.com/user-attachments/assets/2831a110-4ce5-4cae-96f7-142a1ace46c8" alt="drawing" width="600"/> </p>

</details> 

### 1.2. USB reciever firmware (optional)

### 1.2.1. By Windows Software

## 2. Install xpadneo driver on Linux-based distro

### 2.1. Installation

### 2.2. Postinstall configuration


