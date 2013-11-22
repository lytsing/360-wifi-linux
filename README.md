360-wifi-linux
==============

Setting [360 Mobile WIFI](http://wifi.360.cn/) on Linux

*Notes* this just works on 360 wifi version 1, 360 wifi 2 can't use, type: `iw list` , fuck, no response. you can use `lsusb` command to see your devices type:

* ID 148f:5370 Ralink Technology, Corp.
* ID 148f:7601 Ralink Technology, Corp. 
* ID 148f:760b Ralink Technology, Corp. 

The first line is version 1, other is version 2, they need to install driver, see [360 wifi 2 做无线网卡(Linux)](http://blog.lytsing.org/archives/954.html)

(1) It has been tested on fedora 16 (kernel version < 3.6.11).

(2) Linux has a bug of USB 3.0 driver (dmesg | grep "ERROR no room on ep ring"). If it does not work on USB 3.0 slots, you can try the following workaround:

    a. Insert an old USB device (USB 2.0) into the USB slot and then remove it

    b. Insert 360 Mobile WIFI into the slot

    c. Run the script
