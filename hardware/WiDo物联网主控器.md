##WiDo物联网主控器

> Wido是一款轻量化WIFI传感器节点控制器，兼容Arduino Leonardo. 通过Wido你可以轻松对接国内外各大物联网平台，监控环境与设备数据。

![WIDo](http://wiki.dfrobot.com.cn/images/thumb/4/49/DFR0321_Pinout.png/800px-DFR0321_Pinout.png)
Arduino Leonardo兼容设计

支持Micro USB直插供电与编程

外接电源电压范围：7-12v

板载WIFI嵌入式模组，2.4GHz IEEE 802.11 b/g

SPI驱动WIFI模组

板载Micro SD卡槽

PCB 2.4G天线，提供接近手机的WIFI信号

驱动引脚：

WIFI模块—D7(IRQ),D5(VBAT),D10(CS),D14(MISO),D15(SCK),D16(MOSI)

MicroSD —D4(CS),D14(MISO),D15(SCK),D16(MOSI)

PS:4个Arduino Leonardo占用，MicroSD和CC3000都通过SPI驱动，顾有硬件串口资源可扩展其他功能
