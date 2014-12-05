#物联网相关工具

##CoAP

###CoAP-CLI

语言: ``Javascript``

主页: [https://github.com/mcollina/coap-cli](https://github.com/mcollina/coap-cli)

> CoAP的命令行工具

###LibCoAP

语言: ``C``

主页: [http://sourceforge.net/projects/libcoap/](http://sourceforge.net/projects/libcoap/)

> Lightweight application-protocol for devices that are constrained their resources such as computing power, RF range, memory, bandwith, or network packet sizes. This protocol, CoAP, is developed in the IETF working group "CoRE", <http://6lowapp.net>.

示例: 

``起server``

	coap-server

``测试``

    coap-client -m get coap://localhost
