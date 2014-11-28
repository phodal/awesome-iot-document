##WIFI-DUINO

> WiFi-Duino是一个可以接入wifi（或者建立wifi热点）的兼容Arduino系列开发软件的开发板，基于Atmega32U4和HLK-RM04 WiFi模块制作，提供比Arduino Yun更加完善的功能，售价仅需￥169。您可以通过它将您的电路设计和互联网相连，快速开发出物联网应用。

![WIFI-DUINO](http://bcs.duapp.com/blogimbed/wifi-duino/v1_fb.png)

> 和Arduino Yun不同的是，我们提供了板载的稳压芯片，WiFi-Duino可以通过USB接口供电，也可以通过供电插座供电，板载检测器会自动切换电源。外部供电设备可以是AC-to-DC配适器或者电池。配适器的连接方式是通过向板载的电源插座插入一个2.1mm的插头（中心为正）；电池则是直接插入供电端口（Gnd和Vin排针）。

>理论上WiFi-Duino可以在6—15伏内正常工作。然而，如果供电不足7伏，5V排针的供电电压可能会小于5伏，板载插座则有可能不能稳定工作。如果供电大于12伏，稳压器则会过热，板载插座也会受损。所以，推荐的外部电源电压范围是7—12伏。
