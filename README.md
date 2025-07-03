# Gamesir (T4) Nova Lite Linux Guide

This guide will help you deal with:
- pairing issues when gamepad can't reconnect
- inability to switch gamepad mode when connected via dongle
- non-working rumble (vibration) on linux when connected via bluetooth
- missing xbox mode (xinput)

To solve these problems, the following steps can be done:
- Install gamepad firmware version 6300 (which is not in the official application by default)
- Install USB dongle firmware (optional)
- Install and configure the xpadneo driver for a PC on Linux

## 1. Install firmware

You can find the official manual and firmware/software files [here](https://doc.xiaoji.com/zh/t4nlite/detail/1192.html). For some reason, this guide is only available in Chinese.

### 1.1. Gamepad firmware

You can change firmware of this gamepad in two ways: via a smartphone or via a Windows PC.

### 1.1.1. By Gamesir World App

Disclaimer! The author (me) did these steps on an Android device and can't provide instructions for iOS users (it should be the same I think)

Get latest version of Gamesir App from [official website](https://gamesir.com/pages/software-detail)

![Снимок экрана_20250703_233114](https://github.com/user-attachments/assets/550d5377-9ae4-44f8-add7-cff7f173016f)

After installing the application, connect the gamepad to your smartphone. To do this, on gamepad press A + HOME buttons. The HOME button will start flashing yellow around. In the smartphone settings, go to Bluetooth, go to something like "search for devices" where in the list there will be "gamesir nova light"

If the device name is not in the list, it means that the gamepad cannot reconnect to the device that it remembered last. To put the gamepad into pairing mode, press HOME button and *the button below it* for 3 seconds. The backlight will start flashing faster, and you will be able to connect to the gamepad.

Inside the gamesir app, add your gamepad: in the device tab, in the upper right corner, click on the gamepad with plus icon, In the appeared list of devices find "gamesir nova lite"

Now, change your device settings to chinese. Yep, without this step, the application will not display the firmware version we are interested in.

DISCLAIMER: Actually, you can install firmware 4200, which is works well, other firmwares after this version work poorly (except 6300)

### 1.1.2. By Windows Software

### 1.2. USB dongle firmware (optional)

### 1.2.1. By Windows Software

## 2. Install xpadneo driver on Linux-based distro

### 2.1. Installation

### 2.2. Postinstall configuration

## 3. Short how-to about device

