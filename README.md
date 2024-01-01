# EOS-Setup
All setup CLI to configure EOS
<br>
<br>
Here are some of the main apps I use:
<br>
<br>
Brave Browser
```
yay -S brave-bin
```
Steam
```
yay -S steam
```
Discord

```
yay -S discord
```
<br>
## Installing Nvidia Drivers
<https://discovery.endeavouros.com/nvidia/new-nvidia-driver-installer-nvidia-inst/2022/03/>  
<br>
This CLI will automatically install Nvidia drivers for your EOS installation

```
nvidia-inst
```  
<br>
<br>

## Installing envycontrol  
<https://discovery.endeavouros.com/hardware/envy-control/2023/03/>  
<br>
This CLI will install envycontrol which allows you to configure Nvidia optimus profiles  

```
yay -S envycontrol
```  

Then once installed you can configure the Nvidia profile using the following CLI  

```
sudo envycontrol -s <mode>
```  

The current mode options are `integrated`, `hybrid`, `nvidia`  
<br>
<br>
<br>
## Download Gnome Software GUI package manager  
This CLI will install the Gnome Software App
```
sudo pacman -Syu gnome-software-packagekit-plugin gnome-software
```
<br>
<br>

## Install Flatpak support
<https://flatpak.org/setup/EndeavourOS>  
<br>
This CLI will install flatpak  

```
sudo pacman -S flatpak
```

Then we need to add Flathub repository  

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```  

<br>
<br>

## Configure Zen Kernel as default  
This CLI will open up the grub loader in Nano  

```
sudo nano /efi/loader/loader.conf
```  


Then change the content of the loader to include the kernel name as default  

```
default *zen.conf
timeout 5
console-mode auto
reboot-for-bitlocker 1
```  

You can also view the currently running kernel with the following CLI  

```
uname -r
```  

<br>
<br>

## Wallpapers
<https://www.pexels.com/photo/mountain-peaks-during-night-time-3389618/> 
<br>

<br>
<br>

## Gnome Extensions
Here's a list of the best extensions
<br>
<br>
First install the extension manager from Aur
<br>

```
yay -S extension-manager
```
<br>

Now install the following extensions:
<br>
Dash to Dock
<br>
Blur My Shell
<br>
Desktop Cube
<br>
Coverflow Alt-Tab
