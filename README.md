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

