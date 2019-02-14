# OC_gtx1080ti
OC_gtx_1080_ti
original post:https://www.overclock.net/forum/69-nvidia/1627212-how-flash-different-bios-your-1080-ti.html

# how to flash:
Right click on all zip files, choose Properties and Unblock before unzipping them, might be an issue if you don't.

Unzip NVFlash to a folder.

Run an admin command prompt and cd to the folder you made.

Do in command prompt:

To turn protection off so you can flash the BIOS.

$ nvflash64 --protectoff

Then to backup original bios.

$ nvflash64 --save filename.rom

To flash bios.

$ nvflash64 -6 biosfilename.rom

If screen goes black just hit the 'y' key twice, it'll flash and screen will come back on.

Reboot, reinstall Nvidia driver, reboot again.

Unzip this file and run this .bat file after boot to fix TDP limit or add it to your task scheduler to run 60 seconds after boot with the highest privileges. You'll need it to run every boot.
