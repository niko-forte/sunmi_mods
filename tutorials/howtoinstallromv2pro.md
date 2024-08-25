## PLEASE PAY ATTENTION TO THE FOLLOWING STEPS IF YOU DO NOT WANT TO LEAVE YOUR DEVICE UNINVERSABLE
This tutorial IS ONLY for Sunmi V2 Pro

First of all, you must VERY CAREFULLY uncover the device and then locate the test points (see next image)

![](https://github.com/niko-forte/sunmi_mods/blob/main/tutorials/data/TestPoint_1.png)

You will need the following programs:

QPST 2.7 (Includes qfil)
https://www.mediafire.com/file/55ptn3ztgwgzg2m/QPST_2.7.496.zip/file

The firehose programmer:
https://www.mediafire.com/file/sdaturhgquuhu9m/firehose_8917.zip/file

Qualcomm drivers (only if you don't have the installer)
https://www.mediafire.com/file/7u4m6d36spxhrlt/Qualcomm_USB_Drivers.zip/file

Assuming you have all the programs and drivers installed, let's continue
You need to make a bridge with something metallic between the 2 test points
Make sure the bridge is well made and (with the device off) keep the bridge on the test point
And connect the USB cable to the device and to the PC (after opening the Qfil)
It should appear like the following image

![](https://github.com/niko-forte/sunmi_mods/blob/main/tutorials/data/qfil.png)

(it doesn't have to be COM5) that depends on the port on your PC
The important thing is that if Qualcomm HS-USB QDLoader 9008 appears
If it appears like that, you are on the right track. If not, stop and start the whole process again.
select in qfil "flat build" and in the select programmer section select Browser
and look for the downloaded firehose
after you have selected the correct firehose go to
Tools/partition manager, if the following box appears

![](https://github.com/niko-forte/sunmi_mods/blob/main/tutorials/data/confirm.png)

Just select "ok" and after a few seconds the following should appear:

![](https://github.com/niko-forte/sunmi_mods/blob/main/tutorials/data/partitionlist.png)

When the list of partitions appears, you should look for the following 3 partitions:
Boot Devinfo System
Right-click on the partition and click on "manage partition data"
For greater security, I would suggest starting with the devinfo partition
Then the boot partition and finally the system partition
When you click on "manage partition data" you should see the following:

![](https://github.com/niko-forte/sunmi_mods/blob/main/tutorials/data/flash.png)

Click on load image (ONLY IF YOU SELECT THE PARTITIONS INDICATED)
otherwise your device may become unusable
once you do that and remember that you must start with devinfo
click on load image and look for the devinfo.bin file and wait for it to finish, then do the same with the boot (boot.img file) and finally system (system.img file)
once everything is finished close all the boxes, the device should reboot itself
if it doesn't, hold down the power button and the volume down button until it reboots
when it reboots you should see the following

