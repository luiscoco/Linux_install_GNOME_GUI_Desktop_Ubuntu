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

