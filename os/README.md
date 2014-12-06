#物联网相关嵌入式操作系统

> 实时系统（Real-time operating system,RTOS）的正确性不仅依赖系统计算的逻辑结果，还依赖于产生这个结果的时间。实时系统能够在指定或者确定的时间内完成系统功能和外部或内部、同步或异步时间做出响应的系统。因此实时系统应该在事先先定义的时间范围内识别和处理离散事件的能力；系统能够处理和储存控制系统所需要的大量数据。

###Contiki

**相关支持**: ``CoAP``,``TCP/IP网络支持``,``RPL路由``,``6Lowpan 报文压缩``,``Rime无线协议栈``

> Contiki是一个适用于有内存的嵌入式系统的开源的、高可移植的、支持网络的多任务操作系统。包括一个多任务核心、TCP/IP 堆栈、程序集以及低能耗的无线通讯堆栈。Contiki 采用 C 语言开发的非常小型的嵌入式操作系统，运行只需要几K的内存。

Contiki 是一个小型的，开源的，极易移植的多任务电脑操作系统。它专门设计以适用于一系列的内存受限的网络系统，包括从8位电脑到微型控制器的嵌入系统。它的名字来自于托尔·海尔达尔的康提基号。

Contiki只需几kilobyte的代码和几百字节的内存就能提供多任务环境和内建TCP/IP支持。

###LwIP

> LwIP是Light Weight (轻型)IP协议，有无操作系统的支持都可以运行。LwIP实现的重点是在保持TCP协议主要功能的基础上减少对RAM 的占用，它只需十几KB的RAM和40K左右的ROM就可以运行，这使LwIP协议栈适合在低端的嵌入式系统中使用。

> lwIP协议栈主要关注的是怎么样减少内存的使用和代码的大小，这样就可以让lwIP适用于资源有限的小型平台例如嵌入式系统。为了简化处理过程和内存要求，lwIP对API进行了裁减，可以不需要复制一些数据。

###FREERTOS

> FreeRTOS是一个迷你操作系统内核的小型嵌入式系统。作为一个轻量级的操作系统，功能包括：任务管理、时间管理、信号量、消息队列、内存管理、记录功能等，可基本满足较小系统的需要。

> 由于RTOS需占用一定的系统资源(尤其是RAM资源)，只有μC/OS-II、embOS、salvo、FreeRTOS等少数实时操作系统能在小RAM单片机上运行。相对μC/OS-II、embOS等商业操作系统，FreeRTOS操作系统是完全免费的操作系统，具有源码公开、可移植、可裁减、调度策略灵活的特点，可以方便地移植到各种单片机上运行，其最新版本为8.0.0版。

###mbed OS

![mbed OS](./images/mbedos.png)

**相关支持**: ``BLE``,``Celluar``,``WIFI``,``Zigbee``,``6LoWPAN``

> 一款基于ARM Cortex-M处理器的设备所设计的免费操作系统，配有安全、通讯和设备管理模块，支持低功率智能蓝牙标准、2G、3G与CDMA通信技术、Thread、Wi-Fi、802.15.4/6LoWPAN、TLS/DTLS、CoAP、HTTP、MQTT以及轻量级的M2M。而只需32-64kbRAM和256 kb闪存的配置，适合在小设备上运行。

> mbed™ OS is an operating system for IoT devices and is especially well-suited to run in energy constrained environments. The OS includes the connectivity, security and device management functionalities required in every IoT device.

 - Connectivity protocol stack support for Bluetooth® low energy, Cellular, Ethernet, Thread, Wi-fi®,  Zigbee IP, Zigbee NAN, 6LoWPAN
 - Automation of power management
 - Software asset protection and secure firmware updates for device security & management
 - Supports a wide range of ARM Cortex-M based hardware platforms from major MCU vendors
 - Support for OMA Lightweight M2M protocol for device management
 - Updatable and secure devices at the edge capable of additional processing and functionality
 - Banking-class end-to-end IP security across the communication channels through TLS & DTLS 
 - Future proof designs by supporting all the key open standards for connectivity and device management

##emOS

> embOS是一个优先级控制的多任务系统，是专门为各种微控制器应用于实时系统应用的嵌入式操作系统．是一个具有最小RAM和ROM占用的、高速的、多功能的高性能工具。

> 贯穿embOS的整个开发过程，微控制器有限的资源一直是开发者所顾忌的。五年来，该RTOS的内部结构已经被优化为不同客户的不同应用中，以满足工业需要。对不同微控制器的完全源码，使开发者很方便用实时操作系统构建实时程序。embOS是高度模块化的，只有需要的函数才被调用，占用的ROM非常小。 最小的内存占用：1kb ROM,30字节 RAM;由于提供源码文件，你可以用embOS灵活定制系统以满足实际需求。
任务之间可以通过旗语、邮箱和事件安全便利地通讯。

##Salvo

> Salvo™ is the first Real-Time Operating System (RTOS) designed expressly for very-low-cost embedded systems with severely limited program and data memory. With Salvo, you can quickly create low-cost, smart and sophisticated embedded products. Pumpkin™ has currently certified Salvo for use with:

- 8051 family and its derivatives
- ARM® ARM7TDMI® and Cortex™-M3
- Atmel® AVR® and MegaAVR™
- Epson S1C17 family
- Motorola M68HC11
- TI's MSP430 Ultra-Low Power Microcontroller
- Microchip PIC12|14000|16|17|18 PICmicro® MCUs
- Microchip PIC24 MCUs and dsPIC® DSCs
- Microchip PIC32™ MCUs
- TI's TMS320C2000 DSPs

##μC/OS-II

> uC/OS II(Micro Control Operation System Two) 是一个可以基于ROM运行的、可裁减的、抢占式、实时多任务内核，具有高度可移植性，特别适合于微处理器和控制器，是和很多商业操作系统性能相当的实时操作系统(RTOS)。

> 为了提供最好的移植性能，uC/OS II最大程度上使用ANSI C语言进行开发，并且已经移植到近40多种处理器体系上，涵盖了从8位到64位各种CPU(包括DSP)。 uC/OS II可以简单的视为一个多任务调度器，在这个任务调度器之上完善并添加了和多任务操作系统相关的系统服务，如信号量、邮箱等。其主要特点有公开源代码，代码结构清晰、明了，注释详尽，组织有条理，可移植性好，可裁剪，可固化。内核属于抢占式，最多可以管理60个任务。从1992年开始，由于高度可靠性、移植性和安全性，uC/OS II已经广泛使用在从照相机到航空电子产品的各种应用中。

##TinyOS

协议支持: ``CoAP``

[TinyCoAP](http://tinyos.stanford.edu/tinyos-wiki/index.php/CoAP_-13)

> TinyOS是UC Berkeley（加州大学伯克利分校）开发的开放源代码操作系统，专为嵌入式无线传感网络设计，操作系统基于构件（component-based）的架构使得快速的更新成为可能，而这又减小了受传感网络存储器限制的代码长度。

> TinyOS的构件包括网络协议、分布式服务器、传感器驱动及数据识别工具。其良好的电源管理源于事件驱动执行模型，该模型也允许时序安排具有灵活性。TinyOS已被应用于多个平台和感应板中。

###支持硬件

 - Atmel ATmega128, a 8-bit RISC microcontroller.
 - Texas Instruments MSP430 a 16-bit low power microcontroller.
 - Intel XScale PXA271 a 32-bit RISC microcontroller.

##MQX

> Freescale MQX™ RTOS a full-featured complimentary real-time operating system including the MQX™ Kernel, TCP/IP stack (RTCS), embedded MS-DOS file system (MFS), USB host/device stack, and more. The MQX™ multitasking kernel provides pre-emptive scheduling, fast interrupt response, extensive inter-process communication and synchronization facilities. MQX RTOS includes its own peripheral drivers.


