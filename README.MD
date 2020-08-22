I own a Samsung A31, none of the guides that I've followed have worked.
This guide aims to document the process myself.

### Phone Model:
- SM-A315G/DS
- Apparently 'DS' stands for Dual-sim

### Required Files:
- Odin - https://odindownload.com/download/
- Magisk - https://github.com/topjohnwu/Magisk/releases/
- Latest Firmware - https://samfrew.com/model/SM-A315G/region/XSA/

### Unlocking the bootloader:
- Ensure you're not logged into and Samsung or Google accounts
- Settings -> About Phone -> Tap on 'Build number' until you have 'Developer Mode' enabled
- Navigate to Developer mode and turn on 'OEM Unlock'
- Turn off phone -> Hold 'Vol up' + 'Vol Down' -> Plug USB-C Cable from PC into Device
- HOLD Volume up, this will now unlock the bootloader

### Created a patched firmware file:
- Extract the A31 firmware with winrar, 7zip had trouble extracting
- Copy the AP file to your device, should be about 4Gb or so
- Install Magisk Manager
- Launch and tap on 'Install' - > 'Select and Patch a File', select the AP file you transferred
- Magisk will start patching the file, it will generate a file named 'magisk_patched.tar'
- Copy that file back to your computer

### Installing the firmware
- Boot into download mode
- Run Odin
- Check 'AP' and select out patched 'magisk_patched' file
- Check BL, CP, and Home_CSC files, load them from our downloaded firmware folder from, earlier
- Uncheck 'Auto Reboot'

### Bits I'm unsure about - Pending my own testing
- as soon as the phone display turns off, press and hold the Power + Volume Up buttons at the same time. Now when you see your phone’s model on the screen just release all the buttons except the Volume Up. If you miss this step, then you have flash “magisk_patched.img” again.
Now wipe all data by choosing Wipe data/factory reset.
After you device is cleaned, simply click on Reboot.
Now hit on “Start” button and the flashing process will start.


- Press 'Power' + 'Volume Down' to exit download mode. 
- As soon as the screen turns off, immediately press the combo key 'Power' + 'Volume Up' to boot to recovery. 
- Continue pressing the volume up button until you see the stock recovery screen.
- Use the Volume Buttons to Choose Wipe data/factory reset
 
- Now Choose the Reboot System Now and Hold down the Power + Volume Up buttons. As soon as you see the Warning screen, release all the buttons. Your System will now Boot into the System with Magisk

- You need to do this every single time you will reboot the device, Here are the Combinations you need to learn
