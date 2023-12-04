# Linux_install_GUI_Desktop_Ubuntu

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

