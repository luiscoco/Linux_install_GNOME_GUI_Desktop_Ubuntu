# How to install Linux GNOME GUI Desktop in a virtual machine AWS EC2 with Ubuntu image

https://posintech.com/give-your-linux-desktop-a-clean-look/

https://www.youtube.com/watch?v=afpdn636NE0

## 1. Create a Virtual Machine (with Ubuntu image) EC2 in AWS.

We login in AWS

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/f0469218-f921-4274-8af1-7c83337b6742)

We navigate to EC2 virtual machines

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/31becc07-07cb-4430-ad78-11269a3adb64)

We press the "**Launch Instance**" button

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/63f2aadb-0818-4bd5-bad6-f881795c227b)

We set the new VM name

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/b1596307-7daa-4ea5-b39c-ba73b5279a44)

We select the VM immage

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/167ad42e-2a82-48ba-b320-4d2c2b2e202b)

We select the VM type

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/08dd1c97-a58b-4d3e-9514-c0e1b82f4eab)

We generate a Key Pair for accessing with SSH to the VM

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/05a2d877-a1b7-4d87-aa3c-27eba0cc995b)

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/09e92374-09e1-4dfd-85f4-cd6c7e7c97ae)

We place the key pair private file *.pem in the user ssh path "C:/Users/luisc/.ssh/"

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/823eae35-af08-4c4d-b025-59a46b636d4c)

We edit the Network Setting and we add a new inbound rule to access into the VM from Remote Desktop Protocol RDP in port 3389

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/cf99ccce-9272-4d8e-bafe-62ad85896e82)

We configure the storage to 30 Gb

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/a4072774-4b7c-4808-88b5-d427143248e0)

We click on Advanced details to request a **Spot Instance**

We set the Spot options

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/9b2a7c94-d44f-47f2-bafe-0b931457b767)

Finally we launch the instance

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/55973196-5fb7-4c83-93c3-0d20e87ae549)

We navigate to the instance clicking on the VN Id

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/26f52bb9-3f5d-43f4-827b-7d99ba0a1c54)

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/495637f1-cc73-4e4b-9054-201cdf262b14)

We select the instance and we connect to it

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/c4e7c9dc-0715-4ca8-a549-c4d5f7ec8ac0)

We navigate to the **SSH tab**

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/9c9c64da-7dcc-4eac-a143-6ed964e835a2)

We copy the SSH launch connection string 

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/ec3b38c0-4841-483d-9c87-e013d0483d52)

We open the command prompt and we paste the connection string taking into account we have to update the actual .pem file path

ssh -i "C:/Users/luisc/.ssh/mynewkeypairforlinuxvn.pem" ubuntu@ec2-13-39-163-28.eu-west-3.compute.amazonaws.com

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/f539d0f8-72ce-47a4-bf8d-6e275ab36643)

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/5405b3d4-8d09-4b27-b9ff-944773d226fa)

## 2. Then run these commands in the Linux VM in order to setup the XRDP and GENOME GUI Desktop

For Ubuntu server VM run these commands

```
sudo apt-get update

sudo apt install xrdp

sudo systemctl enable xrdp

sudo add-apt-repository ppa:gnome3-team/gnome3

sudo apt-get install gnome-shell ubuntu-gnome-desktop
```

We selet with the **tab** button the **ok** button and press it with the Enter key

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/a9379ce5-b49b-41cc-9a5c-07997e7d621d)

Then set the VM password

```
sudo passwd ubuntu
```

We set the user ubuntu password for example "Luiscoco123456"

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/522bfe39-59bf-4029-b77a-2cbef4172f81)

## 3. Connect the VM via "Remote Desktop Connection"

Set the VM Public IP address 

Set the VM username

Press the connect button

## 4. Inside GNOME GUI Desktop

Run these commands:

```
sudo apt install gnome-tweaks -y

sudo apt install gnome-shell-extensions
```

https://www.youtube.com/watch?v=afpdn636NE0

