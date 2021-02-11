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
3. If eTHR exec from TWRP Recovery please change
   From :
   #!/system/bin/sh
   To :
   #!/sbin/sh
4. Change TARGET_USB to match with your Android USB Host.
5. Change DIR_FILE to directory or to correct storage folder.
6. Copy both files to /system/bin directory
7. Set both permission files to 755 or open terminal to run commands :
   chmod 755 /system/bin/eTHR && chmod 755 /system/bin/mkfs.ext4
8. Connect eTHR to Android with USB OTG
9. Open terminal and run command :
   eTHR
10.Enjoy

Note :
“You can edit or change eTHR file for futher development.”
