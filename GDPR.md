# RUI 4.0


- Install deeptest_RUI4.apk
- Start processing, wait a while, go back, click upper-right corner to check status -> should OK
- OEM unlock in Settings
- Alow ADB debug in Settings
- connect to pc and run `adb reboot bootloader`
- if device STATE is locked, then run `fastboot flashing unlock`
- reboot into fastboot
- `fastboot boot twrp11.img`
- change lang to English -> upper right corner icon -> last tab -> select english -> press button on screen
- `adb push RMX2202_11.C.17_GDPR.zip /data/ota.zip`
- on screen select file and install -> make sure to check "Force install stock rom"

- `adb shell "twrp install /data/ota.zip"` ??
