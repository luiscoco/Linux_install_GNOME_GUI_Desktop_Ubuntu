# Linux_install_GNOME_GUI_Desktop_Ubuntu

https://posintech.com/give-your-linux-desktop-a-clean-look/

https://www.youtube.com/watch?v=afpdn636NE0

1. Create an Ubuntu server Linux VM in Azure

2. Connect the VM via SSH

3. Then run the commands

```
sudo apt-get update

sudo apt install xrdp

sudo systemctl enable xrdp

sudo add-apt-repository ppa:gnome3-team/gnome3

sudo apt-get install gnome-shell ubuntu-gnome-desktop

sudo passwd azureuser
```

4. Connect the VM via "Remote Desktop Connection"

Set the VM Public IP address 

Set the VM username

Press the connect button

5. Inside GNOME GUI Desktop

Run these commands:

```
sudo apt install gnome-tweaks -y

sudo apt install gnome-shell-extensions
```

https://www.youtube.com/watch?v=afpdn636NE0

