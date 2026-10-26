# OpenCore-EFI-Surface-Pro-5-2017-
This is a working EFI for Tahoe (macOS 26) for the Microsoft Surface Pro 5 (2017)
The EFI MAY work for other versions of macOS such as Sequoia (15) or Sonoma (14) but I haven't tried it so do with that what you will.
I have pieced together this EFI with many many hours of research and fiddling

Mostly everything works including the touchscreen and battery status but most importantly the display and graphics; known to normally be a problem with the Intel HD 620. I have set all the frame buffers up and whatnot for the graphics so no other alterations for the graphics should need to be done.

The sound drivers won't work out of the box but with OpenCore Legacy Patcher 3.0.0, audio can be restored pretty easily with the root patches.
To make the touchscreen work, you will need to install Xiashangning's IPTSDaemon (https://github.com/Xiashangning/IPTSDaemon) and restart the Surface. After this touchscreen should work perfectly (if perfectly was basic cursor movement).

Things that don't work are the WiFi and Bluetooth due to no support for the Marvell chips used in this surface. Only other alternative is a USB WiFi adapter compatible with Tahoe from factory or by chris1111's usb wifi drivers (https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter)
