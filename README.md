# eTHR Direct ISP eMMC From Android
This is shell script design for run eTHR Tool from Android terminal like thermux.

Will be better if your device using custom rom with ext2, ext3, ext4, f2fs file kernel support.

Make sure your Android has OTG support before use eTHR.

Instructions :
Part A installation
1. Download eTHR & mke2fs as RAW files
2. Edit eTHR file with text editor
3. If eTHR exec from TWRP Recovery please change
   From :
   #!/system/bin/sh
   To :
   #!/sbin/sh
4. Change TARGET_USB to match with your Android USB Host.
5. Change DIR_FILE to directory or to correct storage folder.
6. Copy both files to /system/bin directory
7. Set both permission files to 755 or open terminal to run commands :
   chmod 755 /system/bin/eTHR && chmod 755 /system/bin/mke2fs
8. Connect eTHR to Android with USB OTG
9. Open terminal and run command :
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
1. Session 1
Commands :
su
eTHR

Mount data with menu 2
Mount system with menu 3 
Then swipe termux screen from left to right & choose [new session]

2. Session 2
Commands :
sudo su
cd /storage && mc

3. Please leave /storage/data & /storage/system before exit from eTHR, otherwise data & system wont umounted.

Finish...

Note :
“You can edit or change eTHR file for futher development.”
