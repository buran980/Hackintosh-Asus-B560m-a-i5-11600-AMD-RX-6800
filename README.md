![image](https://github.com/user-attachments/assets/670a04e1-fd80-4bb3-8f56-c7dcf1ba254f)


Hackintosh EFI folder for Asus Prime B560M-A, i5-11600, AMD Radeon RX 6800.
 
Serial number is replaced with XXXXXXXXXX string, everything other is the same.

1. Extract with 7zip.
2. Use GenSMBIOS-master to generate valid serial, replace it, in original config.plist.
3. Use ProperTree to correct serial and save config.plist 
4. 1. Copy EFI folder into EFI FAT32 partition on usb or ssd installer (size 200 MB is enough)
4. 2. I used virtual machine macOS to create installer (20 GB partition). Check guide on https://dortania.github.io/OpenCore-Install-Guide/
4. 3. 229GB partition was for macOS

It's a bit of trial and error to prepare the installer, i put mine directly on the SSD.

Note:
ACPI's generated with OpCore-Simplify
Tool-master used to dump usb.json (later used to make UTBMap.kext), other kext's  downloaded from https://dortania.github.io/builds

P.S: Not working: 
I have Intel Wi-Fi AX-200 card, provided drivers curently don't work under macOS 15.4 Sequoia
