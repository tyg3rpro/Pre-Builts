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
