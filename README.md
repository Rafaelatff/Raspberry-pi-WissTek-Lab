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

When the process is done, the following screen will appear. Then you can remove the SD card from USB adapter and install the SD card in the Raspberry PI.

![image](https://user-images.githubusercontent.com/58916022/206916945-2fe91646-2e84-4017-a6c6-2324c4ce350c.png)

## Preparing Raspberry PI for use

A few packages needed to be installed. 

After the installation proccess is complete, open the Command Prompt and run a 'pip install serial'. The serial is used by '1_Python_MoT_Requisição.py'.


## Installing AnyDesk

Download [AnyDesk](https://anydesk.com/pt/downloads/linux) installer for linux, copy the file to a USB pen drive and then connect it to the Rasp. Or, copy the AnyDesk installer ('/home/pi/outros'folder, file: anydesk_6.1.1-1armhf.deb) from current image to the new one. Start the installation.

![image](https://user-images.githubusercontent.com/58916022/206922915-d6e95ded-8476-4339-8e5a-05daf08d6536.png)

Authentication is necessary. If you do not set any passwork, check next topic to see how to set a new password. Type the password for authentication and waits until the instalation is finished.

![image](https://user-images.githubusercontent.com/58916022/206923049-4ea0fe71-7616-487e-ac34-ccb7ea956b61.png)

Now, the AnyDesk software will be installed and available to use. To open the software, just click on the AnyDesk icon (top-right border os the screen).

![image](https://user-images.githubusercontent.com/58916022/206923907-8fc9ff43-5906-400f-83f2-2e69e8cb3450.png)

Now AnyDesk is ready to be used.

![image](https://user-images.githubusercontent.com/58916022/206923937-a0a37353-da19-4cff-8fc7-ae2e140c531b.png)

## Add a password to the Raspberry Pi

To add a password to the Raspberry Pi, open the Terminal and type: 'sudo rasp-config'.

![image](https://user-images.githubusercontent.com/58916022/206923128-fd5ca3bf-a5c0-4a09-af1d-a9bfccf1274e.png)

Go to '1 System Options'.

![image](https://user-images.githubusercontent.com/58916022/206923214-cd877a37-eadd-4d2f-899a-2ab6f1f4ef45.png)

Go to 'S3 Password'.

![image](https://user-images.githubusercontent.com/58916022/206923256-d1d4887d-6f0c-484f-a22e-7c3a968b524a.png)

Click 'Ok'.

![image](https://user-images.githubusercontent.com/58916022/206923289-e15d12eb-6633-42b3-8f01-53d7309e8cb2.png)

Type the password.

![image](https://user-images.githubusercontent.com/58916022/206923328-f294f94d-f9b0-4d93-86cf-d1811eaf719d.png)

Click 'Ok' and close the Terminal.

![image](https://user-images.githubusercontent.com/58916022/206923362-b6f58953-369c-442a-96eb-b5e56f8697c8.png)

