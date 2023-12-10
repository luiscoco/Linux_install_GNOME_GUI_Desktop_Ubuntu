# Linux_install_GNOME_GUI_Desktop_Ubuntu

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

![image](https://github.com/luiscoco/Linux_install_GNOME_GUI_Desktop_Ubuntu/assets/32194879/5b35e3d7-27c1-4653-9902-ccf87f67030d)

We select the VM type





## 2. Open RDP Remote Desktop Port 3389



## 3. Connect the VM via SSH



## 4. Then run the commands

```
sudo apt-get update

sudo apt install xrdp

sudo systemctl enable xrdp

sudo add-apt-repository ppa:gnome3-team/gnome3

sudo apt-get install gnome-shell ubuntu-gnome-desktop

sudo passwd azureuser
```

## 5. Connect the VM via "Remote Desktop Connection"

Set the VM Public IP address 

Set the VM username

Press the connect button

## 6. Inside GNOME GUI Desktop

Run these commands:

```
sudo apt install gnome-tweaks -y

sudo apt install gnome-shell-extensions
```

https://www.youtube.com/watch?v=afpdn636NE0

