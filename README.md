# Huawei Matebook D15 (2018, MRC-W10) Hackintosh
## Hardware:
- CPU: Intel Core i5-8250U
- GPU: Intel UHD Graphics 620
- Audio: ALC 256
- RAM: 16GB (1xDDR4 SK Hynix 8GB 2400Mhz & 1xDDR4 Kingston 8GB 2400Mhz)
- Storage: SDD LITEON CV8-8E 256GB & Kingston A400 240GB
- Wi-Fi/BT: Replaced with Broadcom 94352z (FRU 04X6020 Lenovo)
- Touchpad: ELAN 2202 i2c

## Software:
- Bootloader: OpenCore 0.8.3
- Installed system: MacOS⌘ 11.6.8 (20G730) Big Sur
- Tested system's: 10.14.x, 10.15.x, 11.6.x, 12.3.x

## Note for working Bluetooth
- Fix Bluetooth module for OS Mojave - Bigsur: Enable BrcmBluetoothInjector.kext in config.plist, and disable BlueToolFixup.kext
- Fix Bluetooth module for OS Monterey and later: Enable BlueToolFixup.kext in config.plist, and disable BrcmBluetoothInjector.kext
- Do not use these kext's at the same time

## ~~Know issues:~~ Everything works fine!
~~WEB-camera darkness~~
~~Easy fix this problem: clone repo [UVC-Util](https://github.com/jtfrey/uvc-util) and paste in Terminal:~~
~~~
./uvc-util -I 0 -s brightness=80 -s contrast=20
~~~
~~Options **brightness** and **contrast** may have values 0-100~~
- Web Camera works fine with legacy kext (HuaweiWebCam.kext)
## PS2 Map:
- F1 - Brightness Down
- F2 - Brightness Up
- F3 - F16
- F7 - F17
- F9 - F18
- F10 - F19
- PrtScr - F13
- Ins - F20

F13-F19 - These are free keys that can be assigned to specific actions.
When you press "FN", the values correspond to the normal values of the keyboard.
