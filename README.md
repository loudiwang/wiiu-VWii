# vWii Decaffeinator

vWii Decaffeinator allows you to restore your vWii without the need of a NAND Backup  
<b>Please backup your SLCCMPT and OTP before using this tool!</b>  

## How does it work
This uses the fact that the Wii U will redownload many missing files when performing a System Update.  
So this homebrew will remove Files that can be redownloaded and forces a System Update.  
This even works while being on the latest Firmware Version!

## How to use
Choose an option from the menu and confirm with `START`.  
After a mode has finished press any button to launch System Settings where you can perform an update.  
The update folder will be recreated if you deleted it! Make sure to delete it again if you want to block updates  
<br>
<b>Light mode</b>  
This will redownload every essential System Title including all IOS
<br>

<b>Aggressive Mode</b>  
This will remove EVERYTHING!  
Save Data, Installed Channels, ...
<br>

<b>Force Update</b>  
This will force an update which may redownload any missing files
<br>

<b>Regenerate setting.txt</b>  
This will regenerate the setting.txt which is the only file that can't be recovered by any of the other modes.  
The file will be regenerated from the consoles region and serial which can be read from the Wii U mode.
<br>

<b>Advanced options</b>  
This lets you manually configure what should be redownloaded

## Troubleshooting
* <b>Error 105-3102 when trying to update</b>  
    Restart your console and go back into System Settings  
    Now do the update again

* <b>Error 160-0101 when powering on the console</b>  
    You'll get that error if you have a wii disc inserted while having a vWii NAND with missing system files.  
    Remove any inserted Wii discs and power on the console to do a system update.

* <b>Updating with Tiramisu</b>  
    After running the decaffeinator, follow the ["Undo Autobooting into PayloadLoader" steps here](https://wiiu.hacks.guide/#/uninstall-payloadloader?id=undo-autobooting-into-payloadloader).  
    Then restart your console and perform the update.  
    After the update is complete, you can follow [this guide to re-enable autobooting](https://wiiu.hacks.guide/#/tiramisu/autobooting).

## Credits
* Wii U Helpers from the [Nintendo Homebrew Server](https://discord.gg/C29hYvh) for helping me with the Project
* All people who contributed to [wut](https://github.com/devkitPro/wut) and [libiosuhax](https://github.com/wiiu-env/libiosuhax)
* rw-r-r-0644 for helping me with the proc UI loop

## Disclaimer
I am not responsible for any damage done to your console  
Always make a NAND backup before trying dangerous tools  

![alt text](https://i.imgur.com/L6UNR8j.jpg "Main Menu")
![alt text](https://i.imgur.com/vJxtJtM.jpg "Advanced Options")
