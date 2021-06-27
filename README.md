![open core version](https://badgen.net/badge/opencore/0.6.6/green "Open core version")

# LENOVO YOGA X390 CORE I7 - 16GB OPENCORE EFI

⚠️WARNING⚠️
----

I'M NOT RESPONSIBLE FOR ANY DAMAGE THAT HAPPENING DURING USING THIS REPOSITORY

PLEASE FOLLOW DORTANIA OPENCORE INSTALLATION AND USE THIS ONLY FOR REFERENCE 

https://dortania.github.io/OpenCore-Install-Guide/

----

⚠️ANOTHER WARNING⚠️
----

A LOT OF PEOPLE REPORT THEIR LAPTOP UNABLE TO TURN ON (BRICK) AFTER DOING NVRAM RESET

-----

Specification
-----

| Name                  | Value                                                     |
|-----------------------|-----------------------------------------------------------|
| Processor             | 8ᵗʰ Generation Intel ®  Core™ i7-8665U                    |
| Display               | 13.3" FHD (1920 x 1080) IPS, anti-reflective, touchscreen |
| Graphic               | Intel UHD 630                                             |
| Ram                   | 16 GB Soldered                                            |
| Storage               | Samsung SSD PM981                                         |
| Micro SD Card Reader  | Realtek                                                   |
| Wifi + Bluetooth card | Intel ®  9560 802.11AC + Bluetooth 5.1                    |
| Webcam                | via usb internal (720p)                                   |
| I/O                   | 2 USB C 2 USB A Microphone Jack                           |
| Sim card reader       | Yes                                                       |

----

Current compatibility
------

| Name                       | Status       | Notes                                                                                                                           |
|----------------------------|--------------|---------------------------------------------------------------------------------------------------------------------------------|
| CPU                        | 🟢           | Patched with CPUFriend                                                                                                          |
| Graphic Card / Display     | 🟢           |                                                                                                                                 |
| Audio                      | 🟢           |                                                                                                                                 |
| Storage                    | 🔴           | Since there is so much problem opencore + PM981 drive,  i end up to change the drive to SSD Adata XPG SX8200 PRO 256GB M.2 NVMe |
| Sleep                      | 🟡           | No USB power, sometimes sleep broke sound input                                                                                 |
| Power / Battery / Charging | 🟡           | Slow charging, probably need battery patch (Need help!)                                                                         |
| Wifi                       | 🟡           | Hard to correctly connect to 2.4Ghz hotspots. Slower. Kext related                                                              |
| Bluetooth                  | 🟡           | Can't connect to Bluetooth 4.0, Kext related                                                                                    |
| USB                        | 🟢           | Not patched yet                                                                                                                 |
| External Display           | 🟢           | Works both using Thunderbolt usb c or HDMI                                                                                      |
| Pen + Touchscreen          | 🟢           | Touchscreen just feel more natural than using Touchpad (Touchpad gesture enabled)                                               |
| Trackpad                   | 🟡           | Scrolling using trackpad while hovering link will opening that link in browser                                                  |
| Touchpad                   | 🟡           | Touchpad feel unnatural, probably need change to VoodooRMI (Need help!)                                                         |
| Smart Card Reader          | 🟢           |                                                                                                                                 |
| Android USB Tether         | 🟢           |                                                                                                                                 |
| Fn Key                     | 🟢           | Please install YogaSMC app + SystemPreference panel                                                                             |
| Sim Card Reader            | 🔴           |                                                                                                                                 |
| Tablet mode detection      | 🟢           | Please install YogaSMC app + SystemPreference panel                                                                             |
| Battery indicator          | 🟢           |                                                                                                                                 |
----

BIOS/UEFI Configuration
----
- Disabled:
    - Always on USB
    - Wake on LAN
    - Wake on USB
    - Intel TXT
    - Secure Boot
-----

HOW TO USE
----
ONLY FOLLOW THIS IF YOU KNOW WHAT ARE YOU DOING
- Make sure you have same spec above
- Follow BIOS / UEFI Configuration
- Follow dortania opencore installation guide to make usb bootable
- copy paste the EFI folder there
- Follow dortania guide to fill Serial Number and UUID to the config.plist inside EFI folder (If you use ProperTree, don't do clean snapshot!)
- Boot! 

----

Tasks (NEED HELP!)
----
- Battery patch (Hopefully will fix slow charging issue)
- Change VoodooPS2 to VoodooRMI (Hopefully fix unnatural touchpad issue)
- SIM Card reader
- Sleep sometimes broke sound input


----

REFERENCES:
----
Here the list of some reference i use to create this EFI folder
- Thinkpad brightness key fix: https://github.com/acidanthera/BrightnessKeys
- Touchscreen fix: https://github.com/acidanthera/VoodooPS2/tree/2.2.2 (Note: Disable `VoodoInput` and use `VodooInput` from `VoodoPS2Controller` instead) (2ndNote: Only VodooI2C and VoodoI2CHUD)
- Battery indicator fix (Just need to download kext, don’t need to do battery patch): https://github.com/RehabMan/OS-X-ACPI-Battery-Driver
- YogaSMC for some fn key functionality fix: https://github.com/zhen-zen/YogaSMC
-  HoRNDIS for android usb tether.
    - 1 Download and install https://github.com/jwise/HoRNDIS/issues/133#issuecomment-751474467 (I don’t know if this required).
    - Use HoRNDIS kext from here: https://github.com/mendax1234/ThinkpadX390-Opencore-EFI/tree/main/EFI/OC/Kexts/HoRNDIS.kext/Contents\
- Card reader fix: https://github.com/cholonam/Sinetek-rtsx
