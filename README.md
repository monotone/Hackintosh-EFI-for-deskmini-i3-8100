# Hackintosh-EFI-for-deskmini-i3-8100
deskmini+i3-8100的hackintosh（黑苹果）efi 配置


### 文件夹说明

#### EFI
该文件夹下的默认`config.list`配置的是dp4K显示器输出。`config_back.list`是我从别处拿来的应急用的配置（启动不到macOS登录的时候用，在啰嗦模式可能要等比较久的时间）。

#### EFI.hdmi
v2ex上 @LXchienne 提供给我的EFI，我没试成功过。

#### tools
一些辅助工具和文档，有些大的工具就没上传了。

### 目前存在的问题
1. 分辨率默认的和最高的就是4k，再低一级的是`1920*1080`了。
2. 睡眠后唤醒，整个系统会明显变得卡顿。

### BISO

#### 刷bios
参考 https://github.com/damnnfo/DeskMini-110-COM 

#### 安装前设置

These settings work on the Deskmini which does NOT have a COM port. If your Deskmini does have a COM port check for any settings relating to the COM port and ensure that the port is DISABLED.（备注，如果是带COM口的，记得关掉，印象中是serialse port）
1. With the Deskmini’s BIOS page shown (press F2 at startup to enter the UEFI), enter Advanced Mode (F6 or click top right).
  3
2. Click on the Exit tab and select Load UEFI Defaults.
3. From the Advanced options page, click on the CPU Configuration option.
4. •
a. Set the Intel Virtualization Technology to DISABLED. *
b. Click on the small left arrow (top left) to return to the main Advanced
options page.
From the Advanced options page, click on the Chipset Configuration option.
a. Set the VT-d option to DISABLED.*
b. Set the IOAPIC 24-119 Entries option to DISABLED.
c. Click on the small left arrow (top left) to return to the main Advanced
options page.
the Advanced options page, click on the USB Configuration option.
5. From
a. Set the XHCI Hand-off to ENABLED.
b. Click on the small left arrow (top left) to return to the main Advanced
options page.
on the Security Tab on the main UEFI page.
6. Click
a. Set the Secure Boot State option to DISABLED.
b. Click on the small left arrow (top left) to return to the main Advanced
options page.
7. Double-check these settings to make sure that they are correct. Then click on the
Exit tab and select the option Save Changes and Exit. The Deskmini will restart.

### 其他
无线网卡我买的`DW1820A`，某宝到手加接线和天线70RMB。测试过使用`config_back.list`可以直接驱动wifi使用，蓝牙的话，我不需要，所以没弄，看论坛里是可以的。



