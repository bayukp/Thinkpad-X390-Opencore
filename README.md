![open core version](https://badgen.net/badge/opencore/0.6.6/green "Open core version")

# LENOVO YOGA X390 CORE I7 - 16GB OPENCORE EFI

OpenCore Information
----




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