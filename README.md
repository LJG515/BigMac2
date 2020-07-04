This patcher works 2008 Mac Pro 3,1. Mac Pro 2009, 2010, 2012 users may also benefit from this package


Credits

Hax.dylib by ASentientBot.
APFS ROM Patcher by DosDude1.
SPX Big Mac PatchToolX by StarPlayrX.

Credits by no means endorse this product.

This patch tool contains Hax.dylib to assist with running the Installer from Catalina. It also contains APFS ROM Patcher for Macs that do not have the proper firmware to boot APFS volumes.



This patcher constains a preinstall.sh that allows users to run the installer to a HFS+ disk. The installer will erase it as an APFS volume.

usage

`sudo ./preinstall.sh`

SSD installation is recommended and here's why. Always install with -v. You will want to catch the apfs_sealvolume command and turn off the power to your Mac, or if installing to external SSD, simply unplug the SSD. Apple tries to create a sealed snapshot along with an encrypted boot disk. On a Mac Pro 3,1 and possibly other unsupported Macs, this can lead to kernal panics with CoreCrpyto. This unorthodox method eliminates this issue.



The post install for Mac Pro 3,1 fixes AppleHDA Audio, CD/DVD access, and Telemetry that is SSE compatible. If you have upgraded your WiFi and Bluetooth to 802.11ac combo card, you WiFi and BT4 should work out of the box. USB2, USB3, and USBC all work out of the box on Mac Pro with Big Sur.

This patcher container a postinstall.sh

usage

`sudo ./postinstall.sh`



Future plans
Mac OS Standard HFS disk mounting (This is pre HFS+)