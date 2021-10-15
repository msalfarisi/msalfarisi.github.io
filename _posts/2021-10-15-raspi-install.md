---
title: 'Raspberry pi headless installation'
date: 2021-10-15
permalink: /posts/2021/10/raspi-install/
tags:
  - raspi
  - diy
  - science
  - en
---

This article is to document my step-by-step experience in headless installation of raspberry pi. Similar tutorial is available in many other places. I am using a Raspberry Pi 3 Model B with 1 GB RAM, and installing it on Xubuntu 20.04 LTS.

### Installing Raspberry Pi OS on microSD card

1. Download, install and run the [Raspberry Pi Imager](https://www.raspberrypi.com/software/). Installation of the downloaded package can be done as follows:

```shell
sudo dpkg -i imager_1.6.2_amd64.deb
```

2. Insert a microSD card (I used a 32GB one) to the PC.

3. Choose the operating system (**CHOOSE OS** button) and select **Raspberry Pi OS (32-bit)** from the menu.

<img src='/images/blog-20211015-raspi-imager.png' width='60%'>

<img src='/images/blog-20211015-raspi-imager0.png' width='60%'>

4. Choose the microSD card (**CHOOSE STORAGE** button) and select the intended SD card.

5. Click **WRITE** and the installation procedure will start. This process takes several minutes since _Raspberry Pi Imager_ downloads _Raspberry Pi OS_ and burns it to our microSD card.

At this point, the basic installation of the OS is finished. We can plug in the SD card to the Raspberry Pi, connect it to a monitor, keyboard, mouse and power source to boot it up. However, that requires many pheripherals, so I go headless instead.

6. Create an empty file named **ssh** (without file extension) in the root directory (**boot** device) of the card. Raspberry Pi OS will automatically enable SSH (secure socket shell) when it sees this file on its first boot-up. This allows us to access the Pi command line remotely from our PC.

7. Configure a network connection for the Raspberry Pi. I used an ethernet cable to connect the Raspberry Pi to my router.

### Accessing Raspberry Pi through SSH

1. Install PuTTY from the terminal as follows:

```shell
sudo apt-get update
sudo apt-get install putty
```

2. Run PuTTY and enter **raspberrypi** or **raspberrypi.local** as the host name address.

<img src='/images/blog-20211015-raspi-putty.png' width='60%'>

3. Accept if there is any security warning. It is a local connection, and thus there should not be any problem.

4. It will ask for the username and password. The default initial ones are **pi** as username and **raspberry** as password.

<img src='/images/blog-20211015-raspi-putty0.png' width='60%'>

Now we are connected through the terminal. To access the GUI, we need to enable VNC as follows.

### Accessing Raspberry Pi through VNC

1. Launch the configuration setting of the Raspberry Pi using the following command through the PuTTY terminal:

```shell
sudo raspi-config
```

2. Select the **Interface Options**.

<img src='/images/blog-20211015-raspi-putty1.png' width='60%'>

3. Select **VNC** and **Yes** to enable it. Then finish the configuration.

<img src='/images/blog-20211015-raspi-putty2.png' width='60%'>

4. On the PC, download and install [VNC viewer](https://www.realvnc.com/en/connect/download/viewer/):

```shell
sudo dpkg -i VNC-Viewer-6.21.406-Linux-x64.deb
```
5. On the dasboard, launch the **raspberrypi** or **raspberrypi.local**.

<img src='/images/blog-20211015-raspi-vnc.png' width='60%'>

6. Accept if there is any security warning. It is a local connection, and thus there should not be any problem.

7. It will ask for the username and password. The default initial ones are **pi** as username and **raspberry** as password.

<img src='/images/blog-20211015-raspi-vnc0.png' width='60%'>

Now our Raspberry Pi desktop will appear in a window on our PC. We will be able to control everything from here.
