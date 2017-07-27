## Wifi & Video Drivers
### Wifi Drivers
* From console:
  ```bash
  $ sudo apt install wireless-tools
  $ sudo apt install pciutils
  ```
  [Check this link](https://wiki.debian.org/brcmfmac)
* Driver description
  * ## The Broadcom brcmfmac driver
  ```
  This page describes how to enable support for WiFi devices based on the Broadcom BCM43602 chip on Debian systems.
  brcmfmac is a free and open source driver.
  Non-free firmware is required.
  ```
* Installation
  1. Download the firmware from the Linux firmware git repo. (https://git.kernel.org/cgit/linux/kernel/git/firmware/linux-firmware.git/plain/brcm/brcmfmac43602-pcie.bin)
  2. Move this file to the folder `/lib/firmware/brcm/`, creating the folder if necessary.
  3. Reboot the system.
  4. [Configure](https://wiki.debian.org/WiFi/HowToUse) your wireless interface as appropriate.
* Chipset supported
```
Broadcom BCM43602 (PCI ID 14e4:43ba (Supported in 3.19+, 2 GHz device)
```
