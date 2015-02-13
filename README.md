#物联网

> 物联网是新一代信息技术的重要组成部分，其英文名称是：“The Internet of things”。顾名思义，物联网就是物物相连的互联网。这有两层意思：其一，物联网的核心和基础仍然是互联网，是在互联网基础上的延伸和扩展的网络；其二，其用户端延伸和扩展到了任何物品与物品之间，进行信息交换和通信 也就是物物相息。物联网就是“物物相连的互联网”。

##物联网协议

Protocol |	CoAP  |	XMPP |	RESTful HTTP |	MQTT
---------|---------|---------|---------|---------
Transport |	UDP |	TCP |	TCP |	TCP
Messaging |	Request/Response |	Publish/Subscribe Request/Response |	Request/Response |	Publish/Subscribe Request/Response
2G, 3G, 4G Suitability (1000s nodes) | Excellent |	Excellent |	Excellent |	Excellent
LLN Suitability (1000s nodes) | Excellent |	Fair |	Fair |	Fair
Compute Resources | 10Ks RAM/Flash | 10Ks RAM/Flash | 10Ks RAM/Flash | 10Ks RAM/Flash
Success Storied	| Utility Field Area Networks |		Remote management of consumer white goods |	Smart Energy Profile 2 (premise energy management/home services) |	Extending enterprise messaging into IoT applications

###XMPP

XMPP是一种基于标准通用标记语言的子集XML的协议，它继承了在XML环境中灵活的发展性。因此，基于XMPP的应用具有超强的可扩展性。经过扩展以后的XMPP可以通过发送扩展的信息来处理用户的需求，以及在XMPP的顶端建立如内容发布系统和基于地址的服务等应用程 序。而且，XMPP包含了针对服务器端的软件协议，使之能与另一个进行通话，这使得开发者更容易建立客户应用程序或给一个配好系统添加功能。

###MQTT

![mqtt](../images/MQTT.png)

MQTT（Message Queuing Telemetry Transport，消息队列遥测传输）是IBM开发的一个即时通讯协议，有可能成为物联网的重要组成部分。该协议支持所有平台，几乎可以把所有联网物品和外部连接起来，被用来当做传感器和致动器（比如通过Twitter让房屋联网）的通信协议。

![MQTT相关库](./protocol/MQTT.lib.md)
![MQTT相关库介绍](./protocol/MQTT.lib.md)

###CoAP

![coap](../images/coap.jpg)

CoAP是受限制的应用协议(Constrained Application Protocol)的代名词。在最近几年的时间中，专家们预测会有更多的设备相互连接，而这些设备的数量将远超人类的数量。在这种大背景下，物联网和M2M技术应运而生。虽然对人而言，连接入互联网显得方便容易，但是对于那些微型设备而言接入互联网非常困难。在当前由PC机组成的世界，信息交换是通过TCP和应用层协议HTTP实现的。但是对于小型设备而言，实现TCP和HTTP协议显然是一个过分的要求。为了让小设备可以接入互联网，CoAP协议被设计出来。CoAP是一种应用层协议，它运行于UDP协议之上而不是像HTTP那样运行于TCP之上。CoAP协议非常的小巧，最小的数据包仅为4字节。

###RESTful HTTP

REST 指的是一组架构约束条件和原则。满足这些约束条件和原则的应用程序或设计就是 RESTful。

Web 应用程序最重要的 REST 原则是，客户端和服务器之间的交互在请求之间是无状态的。从客户端到服务器的每个请求都必须包含理解请求所必需的信息。如果服务器在请求之间的任何时间点重启，客户端不会得到通知。此外，无状态请求可以由任何可用服务器回答，这十分适合云计算之类的环境。客户端可以缓存数据以改进性能。


###Thread

![thread](../images/thread.jpg)

Thread是一种基于简化版IPv6的网状网络协议，该协议由行业领先的多家技术公司联合开发，旨在实现家庭中各种产品间的互联，以及与互联网和云的连接。Thread易于安装、高度安全，并且可扩展到数百台设备。Thread基于低成本、低功耗的802.15.4芯片组开发。目前正在使用的大量产品，只需一次简单的软件升级，便可支持Thread。

##相关Web技术

##Z-Wave

> Z-Wave是由丹麦公司Zensys所一手主导的无线组网规格，Z-wave联盟(Z-wave Alliance)虽然没有ZigBee联盟强大，但是Z-wave联盟的成员均是已经在智能家居领域有现行产品的厂商，该联盟已经具有160多家国际知名公司，范围基本覆盖全球各个国家和地区。

> Z-Wave是一种新兴的基于射频的、低成本、低功耗、高可靠、适于网络的短距离无线通信技术。工作频带为908.42MHz(美国)~868.42MHz(欧洲)，采用FSK(BFSK/GFSK)调制方式，数据传输速率为9.6 kbps，信号的有效覆盖范围在室内是30m，室外可超过100m，适合于窄带宽应用场合。随着通信距离的增大，设备的复杂度、功耗以及系统成本都在增加，相对于现有的各种无线通信技术，Z-Wave技术将是最低功耗和最低成本的技术，有力地推动着低速率无线个人区域网。

##Zigbee

> ZigBee是基于IEEE802.15.4标准的低功耗局域网协议。根据国际标准规定，ZigBee技术是一种短距离、低功耗的无线通信技术。这一名称（又称紫蜂协议）来源于蜜蜂的八字舞，由于蜜蜂(bee)是靠飞翔和“嗡嗡”(zig)地抖动翅膀的“舞蹈”来与同伴传递花粉所在方位信息，也就是说蜜蜂依靠这样的方式构成了群体中的通信网络。其特点是近距离、低复杂度、自组织、低功耗、低数据速率。主要适合用于自动控制和远程控制领域，可以嵌入各种设备。简而言之，ZigBee就是一种便宜的，低功耗的近距离无线组网通讯技术。

###Websocket

> WebSocket protocol 是HTML5一种新的协议。它是实现了浏览器与服务器全双工通信(full-duplex)。

###SOAP

> 简单对象访问协议是交换数据的一种协议规范，是一种轻量的、简单的、基于XML（标准通用标记语言下的一个子集）的协议，它被设计成在WEB上交换结构化的和固化的信息。

###REST

> 表述性状态转移是一组架构约束条件和原则。满足这些约束条件和原则的应用程序或设计就是RESTful。需要注意的是，REST是设计风格而不是标准。REST通常基于使用HTTP，URI，和XML（标准通用标记语言下的一个子集）以及HTML（标准通用标记语言下的一个应用）这些现有的广泛流行的协议和标准。


###IPv6

> IPv6是Internet Protocol Version 6的缩写，其中Internet Protocol译为“互联网协议”。IPv6是IETF（互联网工程任务组，Internet Engineering Task Force）设计的用于替代现行版本IP协议（IPv4）的下一代IP协议。目前IP协议的版本号是4（简称为IPv4），它的下一个版本就是IPv6。

###6LoWPAN

> IETF 6LoWPAN取得的突破是得到一种非常紧凑、高效的IP实现，消除了以前造成各种专门标准和专有协议的因素。这在工业协议（BACNet、LonWorks、通用工业协议和监控与数据采集）领域具有特别的价值。这些协议最初开发是为了提供特殊的行业特有的总线和链路(从控制器区域网总线到AC电源线)上的互操作性。

###UDP

> UDP协议的全称是用户数据报协议，在网络中它与TCP协议一样用于处理数据包，是一种无连接的协议。在OSI模型中，在第四层——传输层，处于IP协议的上一层。UDP有不提供数据包分组、组装和不能对数据包进行排序的缺点，也就是说，当报文发送之后，是无法得知其是否安全完整到达的。UDP用来支持那些需要在计算机之间传输数据的网络应用。包括网络视频会议系统在内的众多的客户/服务器模式的网络应用都需要使用UDP协议。UDP协议从问世至今已经被使用了很多年，虽然其最初的光彩已经被一些类似协议所掩盖，但是即使是在今天UDP仍然不失为一项非常实用和可行的网络传输层协议。

###uIP

> uIP 由瑞典计算机科学学院(网络嵌入式系统小组)的Adam Dunkels 开发。其源代码由C 语言编写，并完全公开。

> uIP 协议栈去掉了完整的 TCP/IP 中不常用的功能，简化了通讯流程，但保留了网络通信必须使用的协议，设计重点放在了 
IP/TCP/ICMP/UDP/ARP 这些网络层和传输层协议上，保证了其代码的通用性和结构的稳定性。


###DTLS

> DTLS(Datagram Transport Layer Security)即数据包传输层安全性协议。TLS不能用来保证UDP上传输的数据的安全，因此Datagram TLS试图在现存的TLS协议架构上提出扩展，使之支持UDP，即成为TLS的一个支持数据报传输的版本。DTLS 1.0 基于 TLS 1.1, DTLS 1.2 基于TLS 1.2。

###NFC

> NFC近场通信技术是由非接触式射频识别（RFID）及互联互通技术整合演变而来，在单一芯片上结合感应式读卡器、感应式卡片和点对点的功能，能在短距离内与兼容设备进行识别和数据交换。工作频率为13.56MHz.但是使用这种手机支付方案的用户必须更换特制的手机。目前这项技术在日韩被广泛应用。手机用户凭着配置了支付功能的手机就可以行遍全国：他们的手机可以用作机场登机验证、大厦的门禁钥匙、交通一卡通、信用卡、支付卡等等。

###WiFi

> Wi-Fi是一种可以将个人电脑、手持设备（如pad、手机）等终端以无线方式互相连接的技术，事实上它是一个高频无线电信号。[1] 无线保真是一个无线网络通信技术的品牌，由Wi-Fi联盟所持有。目的是改善基于IEEE 802.11标准的无线网路产品之间的互通性。有人把使用IEEE 802.11系列协议的局域网就称为无线保真。甚至把无线保真等同于无线网际网路（Wi-Fi是WLAN的重要组成部分）

#物联网相关平台

##Yeelink

主页: [http://www.yeelink.net/](http://www.yeelink.net/)

> Yeelink团队介绍

> 我们是一群热爱互联网, 创意设计与电子产品的年轻人, 主要成员曾经在国际知名的电信, 家电和互联网公司工作, 
2012年5月正式离职开始Yeelink的创办和研发. 

> 我们是一群热爱生活,憧憬美好未来的年轻人,我们用自己的激情去打造服务生活的联网电子产品及物联网服务. 相信我们在APP, 互联网, 通信和硬件全面的研发能力, 能够为用户带来更加贴心的智能生活方式.

##SiteWhere

> The Open Platform for the Internet of Things ™

> 这个项目提供了一个完整的平台，来管理物联网设备、收集数据并用外部系统进行数据整合。SiteWhere发行版本可以下载或在亚马逊云中使用。它还集成了多个大数据工具，包括MongoDB和ApacheHBase。

主页: [http://www.sitewhere.org/](http://www.sitewhere.org/)


###DeviceHive

> 该项目提供一个支持连接设备到物联网的机器对机器通信框架。它包括支持创建网络易于使用基于web的管理软件、应用安全规则和监控设备。该网站提供内置有DeviceHub的样本项目，而且它也有一个“游乐场”部分，允许用户使用DeviceHub在线去看它是如何工作的。

主页: [http://www.devicehive.com/](http://www.devicehive.com/)

###Devicehub.net
> Devicehub.net描述自己为“物联网的开源支柱”。它是一个基于云的服务，存储物联网相关的数据，提供数据的可视化并允许用户在网页上控制物联网设备。开发者使用该服务创建跟踪健康信息的应用程序，监视孩子的位置，自动化家电，跟踪车辆数据，监测天气等等。

主页: [http://devicehub.net/](http://devicehub.net/)

###IoT Toolkit

> 这个项目背后的组织正使用各种工具工作，来集成多个物联网相关的传感器网络和协议。虽然主要的项目时一个智能对象应用程序，但该组织也工作在一个HTTP对Coap的情景下，一个带有嵌入式软件代理的应用程序框架等等。在硅谷，他们也发起了一个“遇见”组织，面向对物联网开发有情趣的人。

主页: [http://iot-toolkit.com/](http://iot-toolkit.com/)

###Mango(芒果)
> “芒果”自称是“世界上最流行的开源的机器对机器软件”。基于网络的它支持多个平台。它的主要功能包括支持多协议和数据库、元点、用户自定义事件、导入/导出等等。

###Nimbits
> Nimbits可以存储和处理特定的数据类型，数据可以是时间标记的或地理标记的。作为服务的公用平台是可用的，或者你也可以下载这个软件并部署它到谷歌应用引擎、或亚马逊EC2上的J2EE服务器上、或一个树莓派上。它支持多种编程语言，包括Arduino、JavaScript、HTML或Nimbits.io Java库。

###OpenRemote
> OpenRemote为基于家居的爱好者、集成商、分销商和制造商提供了四种不同的集成工具。它支持十几种不同的现有协议，允许用户创建几乎任何类型的智能设备（他们能够想到和使用任何支持java的设备来控制它）。该平台是开源的，但在设计和产品开发过程中，该公司也出售各种支持、电子书等工具来进行帮助。

###ThingSpeak
> ThingSpeak可以处理HTTP请求，并存储和处理数据。这个开放数据平台的主要功能包括开放应用程序、实时数据收集、地理位置数据、数据处理和可视化、设备状态信息和插件。它可以集成多个硬件和软件平台，包括Arduino、树莓派、ioBridge/RealTime.io、Electic lmp、移动和网络应用、社会网络和MATLAB数据分析。除了开源版本，还提供托管服务。


[吊兰-MQTT协议,CoAP协议,WebSocket,物联网协议在线测试](http://mqtt.phodal.com)

## License

![cc](https://i.creativecommons.org/l/by-nc/4.0/88x31.png)

本作品采用[知识共享署名-非商业性使用 4.0 国际许可协议](http://creativecommons.org/licenses/by-nc/4.0/)进行许可。

© 2014 [Phodal Huang](http://www.phodal.com). 