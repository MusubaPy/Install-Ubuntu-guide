# Install-Ubuntu-guide ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
Here you will find a comprehensive guide to installing Ubuntu 18.04.

------

- [1. Ubuntu system requirements](#SysReq)
- [2. Preparing to install Ubuntu](#Prep)
    - [2.1 Downloading the image](#LoadISO)
    - [2.2 Writing the image to a USB key](#WriteISO)
    - [2.3 BIOS setup](#BIOS)
- [3.Installing Ubuntu 18.04](#InstallUbuntu)
    - [3.1 Language selection](#LangSec)
    - [3.2 Loading the system installer](#Loader)
    - [3.3 Language selection](#LanguageAgain)
    - [3.4 Keyboard Layout](#Layout)
    - [3.5 Software](#Software)
    - [3.6 How to partition the disk](#PartDist)
    - [3.7 New Partition Table](#PartTable)
    - [3.8 Creating a bootloader partition](#BootLoad)
    - [3.9 Creating a root partition](#RootPart)
    - [3.10 Creating a home partition](#HomePart)
    - [3.11 Finishing disk partitioning](#FinPart)
    - [3.12 Time Zone](#TZ)
    - [3.13 Creating a user](#CreateUser)
    - [3.14 Installing the system](#InstSys)
    - [3.15 Reboot](#Reboot)
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
- 50 GB (8.6 GB for minimal) of hard-drive space (or USB stick, memory card or external drive but see LiveCD for an alternative approach)
- VGA capable of 1024x768 screen resolution
- Either a CD/DVD drive or a USB port for the installer media
- Internet access is helpful

<a name="Prep"></a>
## 2. Preparing to install Ubuntu

Before we can proceed to install the system, we need to prepare everything. The first thing to do is to download the installation image from the official site.


<a name="LoadISO"></a>
### 2.1 Downloading the image

Open the Ubuntu [website](http://releases.ubuntu.com/18.04/) and download the Desktop version image.

![image](https://user-images.githubusercontent.com/11860297/175909902-edb801ea-8a1e-4014-b0e3-0979c39d792a.png)


<a name="WriteISO"></a>
### 2.2 Writing the image to a USB key

Once the image has been downloaded, it must be burned to an installation medium - a flash drive. 
You can use the Etcher utility or Unetbootin to write it to a Linux flash drive.
To write to a flash drive in Windows, you can use the [Rufus](https://rufus.ie/en/) utility.


<a name="BIOS"></a>
### 2.3 BIOS setup

Most computers will boot from USB automatically. Simply insert the USB flash drive and either power on your computer or restart it. You should see a welcome window prompting you to choose your language and either install or try the Ubuntu desktop.

If your computer doesn’t automatically boot from USB, try holding **F12** when your computer first starts. With most machines, this will allow you to select the USB device from a system-specific boot menu.

- **F12** is the most common key for bringing up your system’s boot menu, but **Escape**, **F2** and **F10** are common alternatives. If you’re unsure, look for a brief message when your system starts - this will often inform you of which key to press to bring up the boot menu.


If automatic booting does not start, you need to set the computer to boot not from your hard drive, but from a newly recorded USB installer. To do this, restart your computer and press **Del**, **F8**, **Shift+F2** or another key combination during the BIOS splash screen to open the BIOS setup menu. 

![image](https://user-images.githubusercontent.com/11860297/175530047-57618fd6-1c2e-4082-bd1c-1677226222b8.png)

Here you need to go to the **Boot** tab, and then in the **Boot device priority** section set your flash drive or DVD to the first place. Then you only need to go to the **Exit** tab and click **Exit & Save settings**.

Go to the [website](https://www.lifewire.com/change-the-boot-order-in-bios-2624528) for more information. 
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

In the menu that opens, select **Install Ubuntu** and the installer will start.

![image](https://user-images.githubusercontent.com/11860297/175869770-c0022d28-4063-413f-86c1-6329e18c11be.png)


<a name="LanguageAgain"></a>
### 3.3 Language selection

By default, the system will select English. You must choose **English**.

Choose a language for your future system:

![image](https://user-images.githubusercontent.com/11860297/175870314-dc2e065b-295d-4a36-8feb-d3822f73d796.png)


<a name="Layout"></a>
### 3.4 Keyboard Layout

Select the default keyboard layout. If you need to change the layout during the installation, you can do it with **Alt+Shift** or **Win+Space**.

By default, the system will select English. You must choose **English**.

If you have a non-standard keyboard, you can select it in the list. Alternately, click **Detect Keyboard Layout** and the system will automatically choose your keyboard. If you need to test your keyboard, use the labeled field.

When you’re ready, click **Continue**.

![image](https://user-images.githubusercontent.com/11860297/175870505-a287b4b9-0576-408f-bf59-ab60db7b2c7d.png)



<a name="Software"></a>
### 3.5 Software


You will be asked What apps would you like to install to start with? The two options are ‘Normal installation’ and ‘Minimal installation’. The first is the equivalent to the old default bundle of utilities, applications, games and media players — a great launchpad for any Linux installation. The second takes considerably less storage space and allows you to install only what you need.

Beneath the installation-type question are two checkboxes; one to enable updates while installing and another to enable third-party software.

- We advise enabling both **Download updates** and **Install third-party software**.
- Stay connected to the internet so you can get the latest updates while you install Ubuntu.
- If you are not connected to the internet, you will be asked to select a wireless network, if available. We advise you to connect during the installation so we can ensure your machine is up to date

![image](https://user-images.githubusercontent.com/11860297/175871775-82c983f5-2bf9-4b96-8dc7-2359a4635ecd.png)


<a name="PartDist"></a>
### 3.6 How to partition the disk

Use the checkboxes to choose whether you’d like to install Ubuntu alongside another operating system, delete your existing operating system and replace it with Ubuntu.

- If Windows is already installed, you can trust the installer to do the partitioning automatically. Choose the **Install Ubuntu alongside Windows Boot Manager**.
- You can wipe the hard drive clean prior to installing Ubuntu by clicking **Erase disk and install Ubuntu**.
- Choose the **Something else** option. Use this to specify your own disk partitions or set other advanced options.

![image](https://user-images.githubusercontent.com/11860297/175872998-c3174ca2-16fd-4677-9888-aabaf57687a3.png)

Options related to side-by-side installation or erasing a previous installation are only offered when pre-existing installations are detected.


<a name="PartTable"></a>
### 3.7 New Partition Table

You may choose to allocate the entire free space to root (swapfile and home will be created automatically under root) or you can separate root, swap and home partitioning. Both methods are fine.

I am showing the steps for creating root, / and home partitions separately. But feel free to use a single partition for all of them.


![image](https://user-images.githubusercontent.com/11860297/175882281-2b811d84-bb8a-417c-b646-f0a3c198160e.png)

Traditionally in Linux it is recommended to create three partitions:
- **/boot** for the boot loader;
- **/** for the operating system itself; 
- **/home** for the user files. 

We will follow this scheme. In principle, you do not have to create the **/boot** partition, but it is advisable if you are going to install multiple Linux distributions.

<a name="BootLoad"></a>
### 3.8 Creating a bootloader partition

To create a partition, select **Free space** and click the **+** (plus) sign button. It will provide you with the option to create a Linux partition. In the window that opens you will need to select the size of the partition. Lately the bootloader has been taking up a lot of space, so it is better to leave at least 300 megabytes.

Choose the size, select **Ext2** as file type and **/boot** as the mount point.

Then click the **"OK"** button.

<a name="RootPart"></a>
### 3.9 Creating a root partition

You are creating the Root partition. Anything above 50 GB is more than sufficient for it. Choose the size, select **Ext4** as file type and **/** (means root) as the mount point.

If the **/boot** and **/home** partitions can be left out, this partition is mandatory. This is where the operating system will be located. If you don't make the **/boot** and **/home** partitions, their files will also be on this partition. 

![image](https://user-images.githubusercontent.com/11860297/175898619-e3e5054e-538a-47de-9932-18fac5535ee5.png)

<a name="HomePart"></a>
### 3.10 Creating a home partition

In the similar fashion, create a Home partition. Allocate it maximum space (in fact allocate it rest of the free space) because this is where you’ll save music, pictures and downloaded files.

![image](https://user-images.githubusercontent.com/11860297/175898853-8fa8681f-19a5-4c5b-abb5-be7d064f2579.png)


<a name="FinPart"></a>
### 3.11 Finishing disk partitioning

Once you are ready with Boot, Root and Home, click on **Install Now**:

![image](https://user-images.githubusercontent.com/11860297/175905456-cb19b34b-c2a1-43e8-978b-c74d137cafea.png)

__>>>>P.S. This image may differ from yours.<<<<__

<a name="TZ"></a>
### 3.12 Time Zone

If you are connected to the internet, your location will be detected automatically. Check your location is correct and click ’Forward’ to proceed.

If you’re unsure of your time zone, type the name of a local town or city or use the map to select your location.

![image](https://user-images.githubusercontent.com/11860297/175906347-4132b1d5-1463-4919-8be3-f4ad0b2e2276.png)

__>>>>P.S. If you’re having problems connecting to the Internet, use the menu in the top-right-hand corner to select a network.<<<<__

<a name="CreateUser"></a>
### 3.13 Creating a user

Enter your name and the installer will automatically suggest a computer name and username. These can easily be changed if you prefer. The computer name is how your computer will appear on the network, while your username will be your login and account name.

Next, enter a password. The installer will let you know if it’s too weak.

![image](https://user-images.githubusercontent.com/11860297/175906792-c8645b0f-63ca-4de6-8fa9-271b948521e8.png)


<a name="InstSys"></a>
### 3.14 Installing the system

The installer will now complete in the background while the installation window teaches you a little about how awesome Ubuntu is. Depending on the speed of your machine and network connection, installation should only take a few minutes.

![image](https://user-images.githubusercontent.com/11860297/175907236-d3feaf51-a7c7-4f7d-aef4-868dd7c5babe.png)


<a name="Reboot"></a>
### 3.15 Reboot

After everything has been installed and configured, a small window will appear asking you to restart your machine. Click on Restart Now and remove either the DVD or USB flash drive when prompted. 

![image](https://user-images.githubusercontent.com/11860297/175907446-47995f9f-105c-4ca7-b8f0-1c971c1d55b6.png)


<a name="Conclusion"></a>
## 4. Conclusions

Congratulations! You have successfully installed the world’s most popular Linux operating system!

It’s now time to start enjoying Ubuntu!

Other versions of Ubuntu are installed in the same way.
