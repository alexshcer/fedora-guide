# Fedora Linux Guide
**Note: Asuming you have installed Fedora of you device**


<pre>
1. Why the freaking wifi driver not working ?
</pre>
> Requirments 
> - Ethernet Cable or Bluetooth Threatening or USB Threatening

Connect your device with either of the connection mentioned above and people using blutooth threatening your bluetooth may not work see below for the solution

- Now you could connect to the internet now you have to enable RPM Fusion reposotories
  - To enable the Free repository, use:
  ```bash
  sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
  ```
  - Optionally, enable the Nonfree repository:
  ```bash
  sudo dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
  ```
 
- Now update the system repository database with
  ```bash
  sudo dnf update
  ```
- Now download the drivers
  - For Broadcom Drivers: 
  ```bash 
  sudo dnf install broadcom-wl
  ```
    **_AND_** reboot your system
  
  - For other drivers:
  ```
  sudo dnf install kmod-wl
  ```
  **_OR_**
  ```
  sudo dnf install akmod-wl
  ```
  reboot your system
  
   **_If Still not working_**
  
   Googlt it

<pre>
2. Why the freaking Bluetooth not working ?
</pre>

- To enable bluetooth:
    ```bash 
    systemctl emable bluetooth
    systemctl start bluetooth
    ```
    
<style>
  *{
  background-color:#0000;
  }
</style>
