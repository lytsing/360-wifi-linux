360-wifi-linux
==============

Setting 360 Mobile WIFI (http://wifi.360.cn/) on Linux

(1) It has been tested on ubuntu 12.04 (kernel version < 3.4.0).

(2) Linux has a bug of USB 3.0 driver (dmesg | grep "ERROR no room on ep ring"). If it does not work on the USB 3.0 slots, you can try the following workaround:

    a. Plug in an old USB device (USB 2.0) into an USB slot and then unplug it

    b. Plug in 360 Mobile WIFI into this slot

    c. Run the script
