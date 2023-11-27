# Zeegby2mqtt 
Compose for run zeegby2mqtt with local broker also running on docker

Used CC2531 stick with coordinator FW from https://github.com/Koenkk/Z-Stack-firmware
If You already have bootloader on Your chip, You can re-flash it using USB without wiring and making debugger tools.   

Using it on windows need to solve some quests with accessing to connected USB device from docker.
Usbipd tool will help with it. You need to install it on host (windows) and on wsl.
Installation instruction can be found here: https://github.com/dorssel/usbipd-win/wiki/WSL-support

Auto-attach device by VID/PID (CC2531):
Full list of TI PIDs can be found on https://devicehunt.com/view/type/usb/vendor/0451

usbipd wsl attach -a -i 0451:16a8
