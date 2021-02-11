# eTHR Direct ISP eMMC From Android
This is shell script design for run eTHR Tool from Android terminal like thermux.

And this only work on older Android version like Kitkat 4.4.4.

But will be better if your device using custom rom with ext2, ext3, ext4, f2fs file kernel support.


If you has newer Android version this shell script will works very well on TWRP Recovery.

Just unpack recovery.img and put eTHR on ~/ramdisk/sbin then repack & flash to your device.

Make sure your Android has OTG support before use eTHR.

Instructions :
1. Download eTHR & mke2fs as RAW files
2. Edit eTHR file with text editor
3. Change TARGET_USB to match with your Android USB Host.
4. Change DIR_FILE to directory or to correct storage folder.
5. Copy both files to /system/bin directory
6. Set both permission files to 755 or open terminal to run commands :
   chmod 755 /system/bin/eTHR && chmod 755 /system/bin/mkfs.ext4
7. Connect eTHR to Android with USB OTG
8. Open terminal and run command :
   eTHR
9. Enjoy

Note :
“You can edit or change eTHR file for futher development.”
