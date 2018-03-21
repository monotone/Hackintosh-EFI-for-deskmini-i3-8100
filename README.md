# Hackintosh-EFI-for-deskmini-i3-8100
deskmini+i3-8100的hackintosh（黑苹果）efi 配置


### 文件夹说明

#### EFI
该文件夹下的默认`config.list`配置的是dp4K显示器输出。`config_back.list`是我从别处拿来的应急用的配置（启动不到macOS登录的时候用，在啰嗦模式可能要等比较久的时间）。

#### EFI.hdmi
v2ex上 @LXchienne 提供给我的EFI，我没试成功过。

### 目前存在的问题
1. 分辨率默认的和最高的就是4k，再低一级的是`1920*1080`了。
2. 睡眠后唤醒，整个系统会明显变得卡顿。

### 其他
无线网卡我买的`DW1820A`，某宝到手加接线和天线70RMB。测试过使用`config_back.list`可以直接驱动wifi使用，蓝牙的话，我不需要，所以没弄，看论坛里是可以的。



