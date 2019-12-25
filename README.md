# Pre-Builts
Pre Built Binaries of Ubuntu Touch for the Samsung Galaxy Note 4

# Working
Wifi 
  - Have to reconnect after every reboot/crash
BT 
  - Has stability issues
Cellular 
  - Shows Signal, not enough testing to know if there are other issues, verify APN settings
Status LED 
  - Flashes Green for notifications
Audio
  - Crashes with YouTube videos but seems to work otherwise
  - Music app (and possibly other media apps) dont work, D-BUS errors

# Not Working
Stylus
  - is detected by kernel and shows events but Unity or MIR is not using it at the moment
Sensors
  - test_sensors shows they are recognized, but the GUI isnt seeing them.
Camera
  - Camera will sometimes take a picture, however it will -ALWAYS- cause the device to crash

# How to Install
1. Download all three .img files for your device [WIP]
  - http://tygercraft.duckdns.org/UBPorts/
### 2. Backup any personal data you wish to save
3. Format /data/ to ext4 (Ubuntu Touch is not compatible with F2FS and will not work if you do not do this step)
4. While in TWRP on your host machine (what you connect your device to) do
   - adb push <path>/<to>/<files>/system.img /data/
   - adb push <path>/<to>/<files>/rootfs.img /data/
5. Install halium-boot.img using TWRP to your boot partition
6. verify last 3 steps successfully completed, retry if they have not
7. Reboot and go through setup process
### The Password for the rootfs is 1234
