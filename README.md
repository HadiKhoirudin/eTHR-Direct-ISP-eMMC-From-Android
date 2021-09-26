# eTHR Direct ISP eMMC From Android
This is shell script design for run eTHR Tool from Android terminal like thermux.

Will be better if your device using custom rom with ext2, ext3, ext4, f2fs file kernel support.

Make sure your Android has OTG support before use eTHR.

Instructions :
Part A installation
1. Download eTHR & mke2fs as RAW files
2. Edit eTHR file with text editor i.e Root Explorer / x-plore (root) etc
3. Change TARGET_USB to match with your Android USB Host from /dev/block/platform... ***USB Host etc.
4. Copy both files to /system/bin directory
5. Set both permission files to 755 or open terminal to run commands :
   chmod 755 /system/bin/eTHR && chmod 755 /system/bin/mke2fs
6. Connect eTHR to Android with USB OTG
7. Open terminal and run command :
   eTHR

Part B Prepairing Termux
1. Download Termux on Playstore
2. Open Thermux
3. Run this command
apt-get install mc
apt-get install git
git clone https://www.github.com/ASHWIN990/Termux-sudo.git
cd Termux-sudo
chmod +x install-sudo.sh
 ./install-sudo.sh

Part C Exec

Commands :
su or sudo su (on termux) [enter]
eTHR [enter]

Finish...

Note :
“You can edit or change eTHR file for futher development.”
