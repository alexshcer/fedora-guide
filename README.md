# Fedora Linux Guide
**Note: Asuming you have installed Fedora of you device**


```
1. Why the freaking wifi driver not working ?
```
> Requirments 
> - Ethernet Cable or Bluetooth Threatening or USB Threatening

Connect your device with either of the connection mentioned above and people using blutooth threatening your bluetooth may not work see below for the solution

Now you could connect to the internet now you have to enable RPM Fusion reposotories :
  <pre>sudo dnf install \
  https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm</pre>
