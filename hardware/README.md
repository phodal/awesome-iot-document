#物联网相关开源硬件

##Arduino

语言: ``Processing``,``C++``,``C``

> Arduino 是一款便捷灵活、方便上手的开源电子原型平台，包含硬件（各种型号的 arduino板）和软件（arduino IDE。她适用于艺术家、设计师、爱好者和对于“互动”有兴趣的朋友们。 

![Arduino](../images/arduino.jpg)

> Arduino，是一个基于开放原始码的软硬体平台，构建于开放原始码simple I/O介面版，并且具有使用类似Java，C语言的Processing/Wiring开发环境。 

> Arduino能通过各种各样的传感器来感知环境，通过控制灯光、马达和其他的装置来反馈、影响环境。板子上的微控制器可以通过Arduino的编程语言来编写程序，编译成二进制文件，烧录进微控制器。对Arduino的编程是利用 Arduino编程语言 (基于Wiring)和 Arduino开发环境(based on Processing来实现的。基于Arduino的项目，可以只包含Arduino，也可以包含Arduino和其他一些在PC上运行的软件，他们之间进行通信 (比如 Flash, Processing, MaxMSP)来实现。

[Arduino Yun](./ArduinoYun.md)

> Arduino Yún是Linux与Arduino相结合的WiFi产品。Yún就是汉语中的”云“，目的是让该板子可轻松连接到复杂的网络服务。Arduino Yún是基于ATMEGA32U4和Atheros的AR9331，Atheros的处理器支持OpenWRT的名为Linino的Linux发行版，Arduino Yún已内置以太网和WiFi的支持，USB-A端口、Micro-SD卡插槽、20个数字输入/输出引脚（其中7个可作为PWM输出为模拟输入和12）、一个16 MHz晶体振荡器、一个微型USB连接、一个ICSP头和一个复位按钮。

##Raspberry Pi 

语言: Any
主要有:``Python``,``C#``,``Ruby``

![RaspberryPi](../images/rpi.jpg)

> 树莓派(raspberry pi)，是一款基于linux系统的、只有一张信用卡大小的卡片式计算机。研发树莓派的最初目的是通过低价硬件及自由软件来推动在学校的基础的计算机学科教育，但很快树莓派就得到计算机和硬件爱好者青睐；他们用它学习编程，并创造出各种各样新奇的、风靡一时的软硬件应用。

> 在接口方面，Raspberry Pi提供了可供键鼠使用的USB接口，此外还有快速以太网接口、SD卡扩展接口以及1个HDMI高清视频输出接口，可与显示器或者TV相连。

##Spark Core

语言: ``Processing``,``C++``,``C``

[Spark Core](./SparkCore.md)

> Spark 的核心芯片（Spark Core）采用兼容 Arduino 的 ARM Cortex-M3 平台，搭载一块 德州仪器（TI）CC3000 WiFi 芯片。一切的开始是你再也不用连接 USB 线到电脑，而只需通过 WiFi 即可刷入代码。更重要的是，他们提供了一个免费的云服务，类似非硬件的云服务 Heroku 那样，可以让使用核心板块的自定义程序托管在上面。开发者们可以立即测试自己产品的效果。

##WIFI-DUINO

> WiFi-Duino是一个可以接入wifi（或者建立wifi热点）的兼容Arduino系列开发软件的开发板，基于Atmega32U4和HLK-RM04 WiFi模块制作，提供比Arduino Yun更加完善的功能，售价仅需￥169。您可以通过它将您的电路设计和互联网相连，快速开发出物联网应用。

![WIFI-DUINO](http://bcs.duapp.com/blogimbed/wifi-duino/v1_fb.png)

> 和Arduino Yun不同的是，我们提供了板载的稳压芯片，WiFi-Duino可以通过USB接口供电，也可以通过供电插座供电，板载检测器会自动切换电源。外部供电设备可以是AC-to-DC配适器或者电池。配适器的连接方式是通过向板载的电源插座插入一个2.1mm的插头（中心为正）；电池则是直接插入供电端口（Gnd和Vin排针）。

>理论上WiFi-Duino可以在6—15伏内正常工作。然而，如果供电不足7伏，5V排针的供电电压可能会小于5伏，板载插座则有可能不能稳定工作。如果供电大于12伏，稳压器则会过热，板载插座也会受损。所以，推荐的外部电源电压范围是7—12伏。



#物联网相关闭源硬件


#未知

[WiDo物联网主控器](./WiDo.md)

[WIFI-DUINO](./WIFI-DUINO.md)

[Seeeduino Cloud](./SeeeduinoCloud.md)

[LinkIt One](./LinkItOne.md)