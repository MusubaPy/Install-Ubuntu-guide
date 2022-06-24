# Install-Ubuntu-guide-oos [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)]
Here you will find a comprehensive guide to installing Ubuntu 18.04 as the only operating system

------

- [1. Ubuntu system requirements](#SysReq)
- [2. Preparing to install Ubuntu](#Prep)
    - [2.1 Downloading the image](#LoadISO)
    - [2.2 Writing the image to a USB key](#WriteISO)
    - [2.3 BIOS setup](#BIOS)
- [3.Installing Ubuntu 18.04](#InstallUbuntu)
    - [3.1 Language selection](#LangSec)
    - [3.2 Loading the system installer](#Loader)
    - [3.3 Loading the Live System](#LoadLS)
    - [3.4 Start the installer](#Installer)
    - [3.5 Language selection](#LanguageAgain)
    - [3.6 Keyboard Layout](#Layout)
    - [3.7 Software](#Software)
    - [3.8 How to partition the disk](#PartDist)
    - [3.9 New Partition Table](#PartTable)
    - [3.10 Creating a bootloader partition](#BootLoad)
    - [3.11 Creating a root partition](#RootPart)
    - [3.12 Creating a home partition](#HomePart)
    - [3.13 Finishing disk partitioning](#FinPart)
    - [3.14 Time Zone](#TZ)
    - [3.15 Creating a user](#CreateUser)
    - [3.16 Installing the system](#InstSys)
    - [3.17 Reboot](#Reboot)
    - [3.18 Booting a New System](#BootNewSys)
    - [3.19 Getting to know your system](#Welcome)
    - [3.20 Configuring Livepatch](#Livepatch)
    - [3.21 Privacy](#Privacy)
    - [3.22 Installing applications](#AppInstall)
- [4. Conclusions](#Conclusion)

------
<a name="SysReq"></a>
## 1. Ubuntu system requirements

You’ll need to consider the following before starting the installation:

- Connect your laptop to a power source.
- Ensure you have at least 25 GB of free storage space, or 5 GB for a minimal installation.
- Have access to either a DVD or a USB flash drive containing the version of Ubuntu you want to install.
- Make sure you have a recent backup of your data. While it’s unlikely that anything will go wrong, you can never be too prepared.

Minimal system requirements:
- 2 GHz dual core processor
- 4 GiB RAM (system memory)
- 25 GB (8.6 GB for minimal) of hard-drive space (or USB stick, memory card or external drive but see LiveCD for an alternative approach)
- VGA capable of 1024x768 screen resolution
- Either a CD/DVD drive or a USB port for the installer media
- Internet access is helpful

<a name="Prep"></a>
## 2. Preparing to install Ubuntu

Before we can proceed to install the system, we need to prepare everything. The first thing to do is to download the installation image from the official site.


<a name="LoadISO"></a>
### 2.1 Downloading the image

Open the Ubuntu [website](http://releases.ubuntu.com/18.04/) and download the Desktop version image.

<a name="WriteISO"></a>
### 2.2 Writing the image to a USB key

Once the image has been downloaded, it must be burned to an installation medium - a flash drive. 
You can use the Etcher utility or Unetbootin to write it to a Linux flash drive.
To write to a flash drive in Windows, you can use the Rufus utility.


<a name="BIOS"></a>
### 2.3 BIOS setup

Most computers will boot from USB automatically. Simply insert the USB flash drive and either power on your computer or restart it. You should see a welcome window prompting you to choose your language and either install or try the Ubuntu desktop.

If your computer doesn’t automatically boot from USB, try holding **F12** when your computer first starts. With most machines, this will allow you to select the USB device from a system-specific boot menu.

- **F12** is the most common key for bringing up your system’s boot menu, but **Escape**, **F2** and **F10** are common alternatives. If you’re unsure, look for a brief message when your system starts - this will often inform you of which key to press to bring up the boot menu.


If automatic booting does not start, you need to set the computer to boot not from your hard drive, but from a newly recorded USB installer. To do this, restart your computer and press **Del**, **F8**, **Shift+F2** or another key combination during the BIOS splash screen to open the BIOS setup menu.
![image](https://user-images.githubusercontent.com/11860297/175530047-57618fd6-1c2e-4082-bd1c-1677226222b8.png)


<a name="InstallUbuntu"></a>
## 3.Installing Ubuntu 18.04

Next, need to reboot your computer and we will go straight to installing the operating system.

<a name="LangSec"></a>
### 3.1 Language selection

Immediately after the reboot you will see this window:

![image](https://user-images.githubusercontent.com/11860297/175529993-626c86e6-e4ef-4b8b-b2c3-7c78b04a2e45.png)

You can skip this step and Ubuntu installation will start immediately in English, but it is better to press any button and select English.

<a name="Loader"></a>
### 3.2 Loading the system installer

In the menu that opens, select Install Ubuntu and the installer will start.

<a name="LanguageAgain"></a>
### 3.3 Language selection


<a name="Layout"></a>
### 3.4 Keyboard Layout
<a name="Software"></a>
### 3.5 Software
<a name="PartDist"></a>
### 3.6 How to partition the disk
<a name="PartTable"></a>
### 3.7 New Partition Table
<a name="BootLoad"></a>
### 3.10 Creating a bootloader partition


<a name="RootPart"></a>
### 3.11 Creating a root partition
<a name="HomePart"></a>
### 3.12 Creating a home partition
<a name="FinPart"></a>
### 3.13 Finishing disk partitioning
<a name="TZ"></a>
### 3.14 Time Zone
<a name="CreateUser"></a>
### 3.15 Creating a user


<a name="InstSys"></a>
### 3.16 Installing the system
<a name="Reboot"></a>
### 3.17 Reboot
<a name="BootNewSys"></a>
### 3.18 Booting a New System
<a name="Welcome"></a>
### 3.19 Getting to know your system
<a name="Livepatch"></a>
### 3.20 Configuring Livepatch
<a name="Privacy"></a>
### 3.21 Privacy
<a name="AppInstall"></a>
### 3.22 Installing applications



<a name="Conclusion"></a>
## 4. Conclusions
