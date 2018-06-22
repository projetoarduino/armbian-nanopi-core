DTB to use on armbian distro to work with nano pi core

Install

Burn SD with this image

https://dl.armbian.com/nanopineo/Ubuntu_xenial_next.7z

Get the simple device tree sun8i-h3-nanopi-neo.dtb on repository

and 

cp sun8i-h3-nanopi-neo.dtb /boot/dtb-4.14.14-sunxi/


Only for information

I get DTB file from nano pi air decompile and put only network modification to enable ethernet

dtc -O dtb -o sun8i-h3-nanopi-neo.dtb neo.dts 
cp sun8i-h3-nanopi-neo.dtb /boot/dtb-4.14.14-sunxi/

This Devicetree enable

MMC
Ethernet
SOUND
USBhost
And other hardwares