# Raspberry-pi-WissTek-Lab
Repositorie created to show the steps for preparing the Raspberry Pi 3 to work as border element (gateway).

## Preparing O.S.

Fist, go to [Raspberry Pi website](https://www.raspberrypi.com/software/) and download the Raspberry Pi Imager.

![image](https://user-images.githubusercontent.com/58916022/206914305-4204a2fc-9f7e-4e4d-8890-0e1fe538d26b.png)

Install and Run the Raspberry Pi Imager. Click in 'CHOOSE OS'.

![image](https://user-images.githubusercontent.com/58916022/206914367-410b9d71-65e5-4eea-a046-e0985d64c63c.png)

Go to 'Raspberry PI OS (other)'. Do not choose the latest option (Debian Bullseye), since AnyDesk do not work well in this version. Let's keep the same OS as the current image running in the original SD card of the Raspberry. 

![image](https://user-images.githubusercontent.com/58916022/206914417-85d615eb-ee86-4042-ab62-8766cbb351ae.png)

To check the OS system on Raspberry, I opened the Terminal and typed 'lsb_release -a'.

![image](https://user-images.githubusercontent.com/58916022/206915427-95c49dfa-86cc-4900-a61c-03bc9bbb2cab.png)

Choose the 'Raspberry PI OS (Legacy)' that uses a port of Debian Buster with security updates and desktop environment.

![image](https://user-images.githubusercontent.com/58916022/206915321-14d82ca2-b6c3-474c-8ae6-3c8ed9cf8238.png)

Connect the uSD card through the USB port of the computer. I used same adapter of my 3D printer. 

![image](https://user-images.githubusercontent.com/58916022/206915796-929ea803-7113-4b8d-9cfb-2f54ed26a27b.png)

Click at the 'CHOOSE STORAGE' button.

![image](https://user-images.githubusercontent.com/58916022/206915852-155ff669-befa-4129-b2b1-c87e045416f3.png)

Selected the SD card.

![image](https://user-images.githubusercontent.com/58916022/206915899-c3156877-235d-4be5-8d70-bbaac0bead5d.png)

Click at 'WRITE' button.

![image](https://user-images.githubusercontent.com/58916022/206915927-7be9d9b1-7d0b-4aaf-9e9c-fa524774cdf6.png)

A warning message will appear informing you that all existing data on that SD card will be erased. Confirm your choice by clicking at 'YES' button.

![image](https://user-images.githubusercontent.com/58916022/206915971-8f3fb366-85a6-40e7-a809-71c95edd7322.png)

Just wait until the writing is done.

![image](https://user-images.githubusercontent.com/58916022/206916297-fc7c2832-a381-45ef-be5f-f4bfc6408976.png)






