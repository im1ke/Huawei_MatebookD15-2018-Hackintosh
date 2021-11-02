# Huawei Matebook D15 (2018, MRC-W10) Hackintosh
## Hardware:
- CPU: Intel Core i5-8250U
- GPU: Intel UHD Graphics 620
- Audio: ALC 256
- RAM: 1xDDR4 SK Hynix 8GB 2400Mhz
- Storage: SDD LITEON CV8-8E 256GB & Kingston A400 240GB
- Wi-Fi/BT: Replaced with Broadcom 94352z (FRU 04X6020 Lenovo)
- Touchpad: ELAN 2202 i2c

## Software:
- Bootloader: OpenCore 0.7.5
- Installed system: MacOS⌘ 11.6.1 (20G224) Big Sur
- Tested system's: MacOS 10.14.x, MacOS 10.15.x
- Ready to Monterey (Not tested)

## Know issues:
- WEB-camera darkness
- Easy fix this problem: clone repo [UVC-Util](https://github.com/jtfrey/uvc-util) and paste in Terminal:
~~~~
./uvc-util -I 0 -s brightness=80 -s contrast=20
~~~~
- Options **brightness** and **contrast** may have values 0-100 
## PS2 Map:
- F1 - Brightness Down
- F2 - Brightness Up
- F3 - F16
- F7 - F17
- F9 - F18
- F10 - F19
- Ins - F13
- PrtScr - F20

F13-F19 - These are free keys that can be assigned to specific actions.
When you press "FN", the values correspond to the normal values of the keyboard.
