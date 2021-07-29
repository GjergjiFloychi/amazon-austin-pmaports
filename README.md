# amazon-austin-pmaports postmarketos
Working ebuild for installing postmarketos on the Amazon Fire 7 HD (2017) codename Austin

Amazon Fire 7 (2017) postmarketOS
Armv7l
Mediatek MT8127
Mali-450MP4
600x1024 display
1GB RAM
Linux 3.10.54

What seems to work:

Boot
Touch screen
Battery percentage
Usb internet
OTG usb
Wayland, Mate, Xfce4, Lxde, Sxmo, i3wm

Does NOT work:

Wifi & Bluetooth (no drivers)
GPU acceleration (drivers do not work)
Audio
Sleep and fully turning off the display
Screen rotation
Wifi adapter does not work even with drivers and kernel support, mobo support issue(?)
FDE
Cameras
You tell me

Special options:
*Must be flashed to USERDATA partition as system partition is too small

msm-fb-refresher packaged is added to the depends to make the screen refresh.
After flashing the device must be booted into recovery once. From the recovery it is to be powered off and booted and then as normal. This is because the device depends on the AMONET exploit which is applied by twrp after every flash.
