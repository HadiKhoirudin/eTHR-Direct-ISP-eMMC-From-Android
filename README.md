# eTHR Direct ISP eMMC From Android
This is shell script design for run eTHR Tool from Android terminal like thermux.

Will be better if your device using custom rom with ext2, ext3, ext4, f2fs file kernel support.

Make sure your Android has OTG support before use eTHR.

Instructions :
Part A installation
1. Download eTHR & mke2fs as RAW files
2. Copy both files to /system/bin directory
3. Set both permission files to 755 or open termux to run commands :

   chmod 755 /system/bin/eTHR && chmod 755 /system/bin/mke2fs

4. Connect eTHR to Android with USB OTG
5. Open termux and run command :

   sudo su [enter]

   eTHR [enter]

Part B Prepairing Termux
1. Download Termux on Playstore
2. Open Thermux
3. Run this command

apt-get update

apt-get install mc

apt-get install git

git clone https://www.github.com/ASHWIN990/Termux-sudo.git

cd Termux-sudo

chmod +x install-sudo.sh

 ./install-sudo.sh

Finish...

Note :
“You can edit or change eTHR file for futher development.”
