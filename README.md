Copyright (C) 2019 The LineageOS Project

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Device Tree for SHIFT5me
===========================================

The SHIFT5me is a budget smartphone from SHIFTPHONES.
It was released in late 2018.

Basic   | Spec Sheet
-------:|:-------------------------
Chipset | MediaTek Helio X27
CPU     | Deca-core 1.6/2/2.6 GHz MT6797X (64 bit)
GPU     | Mali-T800 MP4
Memory  | 3 GB RAM LPDDR3
Shipped Android Version | 8.0
Storage | 32 GB eMMC 5.1
MicroSD | Up to 256 GB
Battery | Li-Ion 2430 mAh battery
Display | 1080 x 1920 pixels, 4.97 inches (~443 ppi pixel density)
Camera  | 16 MP, autofocus, LED flash

![SHIFT5me](https://shop.shiftphones.com/media/catalog/product/cache/9/image/600x600/9df78eab33525d08d6e5fb8d27136e95/m/a/magento_produktbilder_shop_shift5me.jpg "SHIFT5me")

TODO:
-----

 * Investigate stock MTK RIL jars, likely needed for IMS/VT

 * Immediately bring up display in recovery
   https://review.lineageos.org/c/LineageOS/android_bootable_recovery/+/244379

DONE:
 * Add support for MediaTek dtbo images  
   https://review.lineageos.org/c/LineageOS/android_vendor_lineage/+/234759
 * Remove duplicated genfs context from system image  
   https://review.lineageos.org/#/c/LineageOS/android_device_lineage_sepolicy/+/224447 (changed in stock vendor.img)
 * Add support for 'resize' flag in fstab (--> resize2fs)  
   https://review.lineageos.org/#/c/LineageOS/android_system_core/+/234734
 * Forcibly add default AOSP WebView provider  
   https://review.lineageos.org/c/LineageOS/android_frameworks_base/+/224757
 * Apply lzma compression for target files in OTA payload  
   https://review.lineageos.org/c/LineageOS/android_build/+/244160
