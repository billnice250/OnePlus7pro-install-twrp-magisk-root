# OnePlus7pro-install-twrp-magisk-root

##Installing TWRP recovery on the Oneplus 7 pro on Android 10(Q)
==============================================================

- Step 1:
  make sure "USB degubing" and "OEM unlocking"( bootloader unlocking) is enabled on your phone
  and it is charged above at least 50%.

- Step 2:
  connect your phone on a computer and transfer the zip file included on phone storage.
  PS: the zip referred is "twrp-3.3.1-74-guacamole-unified-installer-mauronofrio.zip"
  and all the zips you want to install after like the latest versions of "Magisk,Youtube vanced, etc".
- Step 3: putting your phone in bootloader mode(fastboot mode).
  - doing it manuary by pressing a combination of power button or vol buttons
  - Suggested method: adb installed
      1)connected your phone on a computer and type in the terminal(in the PATH of adb files):
         $ adb devices //to be sure that the computer can detect your phone correctly (you should see its id_num displayed)
      1) $ adb reboot bootloader //should reboot the device in fastboot mode in few seconds.
- Step 4: while phone is fastboot mode
  - test: 
     $ fastboot devices //to make sure it is discovered correctly.
  -booting twrp(not installing):
     $ fastboot boot twrp-3.3.1-74-guacamole-unified-Q-mauronofrio.img

**wait for the device to boot into "twrp recorvery" (around 10s)**

- Step 5:
  - tap on "install" and select the zip file "twrp-3.3.1-74-guacamole-unified-installer-mauronofrio.zip" and reboot after the installation  is completed.
  - reboot into recovery again(twrp should be default this time) and install "Magisk___.zip"


**Now TWRP is fully installed and your device is rooted**

After this you can flash all the other files you need.

Installation guide by [Bill Nice G. Havugukuri](https://blog.billnice.it)
