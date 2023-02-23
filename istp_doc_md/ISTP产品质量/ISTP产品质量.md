# ISTP产品质量

## 1. 功能性

### 1.1. 协议识别

#### 1.1.1. 功能说明

流量经过ISTP，通过协议五元组信息，协议字段相关内容，识别是否为该种协议

#### 1.1.2. 发布的标准

协议识别功能包含3种识别方式，分别为AI识别，端口识别，代码识别。

> AI识别：共计100种协议，协议范围如下

| **序号** | **识别方式** | **协议名称**                     |
| ------ | -------- | ---------------------------- |
| 1      | AI识别     | 853                          |
| 2      | AI识别     | BACnet                       |
| 3      | AI识别     | Beckhoff\_AMS\_ADS           |
| 4      | AI识别     | C37.118\_1PMU\_TCP           |
| 5      | AI识别     | C37.118\_1PMU\_UDP           |
| 6      | AI识别     | CIP                          |
| 7      | AI识别     | CoAP                         |
| 8      | AI识别     | COTP                         |
| 9      | AI识别     | DHCP                         |
| 10     | AI识别     | DICOM\_Echo                  |
| 11     | AI识别     | DNP3                         |
| 12     | AI识别     | ENIP                         |
| 13     | AI识别     | FF\_LR\_UDP                  |
| 14     | AI识别     | Focas                        |
| 15     | AI识别     | GDW\_376.1                   |
| 16     | AI识别     | GE\_EGD                      |
| 17     | AI识别     | GE\_SRTP                     |
| 18     | AI识别     | Gryphon                      |
| 19     | AI识别     | HartIP\_TCP                  |
| 20     | AI识别     | HartIP\_UDP                  |
| 21     | AI识别     | HL7                          |
| 22     | AI识别     | HollySys\_DCS\_MACS          |
| 23     | AI识别     | HollySys\_LK-UDP\_6000       |
| 24     | AI识别     | HollySys\_PLC                |
| 25     | AI识别     | HoneyWell                    |
| 26     | AI识别     | HSRP                         |
| 27     | AI识别     | HTTP                         |
| 28     | AI识别     | ICCP                         |
| 29     | AI识别     | IEC103                       |
| 30     | AI识别     | IEC60870-5-104               |
| 31     | AI识别     | IEC61850-MMS                 |
| 32     | AI识别     | ifix2ifix                    |
| 33     | AI识别     | ISAKMP                       |
| 34     | AI识别     | KerberosAuthenticationSystem |
| 35     | AI识别     | KingView\_TCP\_2001          |
| 36     | AI识别     | LDAP\_TCP\_SASL\_Digest      |
| 37     | AI识别     | LON                          |
| 38     | AI识别     | LPD                          |
| 39     | AI识别     | Microsoft\_SQL\_Server       |
| 40     | AI识别     | MITSUBISHI MELSEC\_Q\_UDP    |
| 41     | AI识别     | MITSUBISHI\_MELSEC\_L\_TCP   |
| 42     | AI识别     | Modbus\_ASCII                |
| 43     | AI识别     | Modbus\_RTU                  |
| 44     | AI识别     | Modbus\_TCP                  |
| 45     | AI识别     | Modbus\_UDP                  |
| 46     | AI识别     | Modbus\_UMAS                 |
| 47     | AI识别     | MOXA\_E1242\_UDP             |
| 48     | AI识别     | MQTT                         |
| 49     | AI识别     | Omron\_FINS\_TCP             |
| 50     | AI识别     | Omron\_FINS\_UDP             |
| 51     | AI识别     | OPC\_DA                      |
| 52     | AI识别     | OPC\_UA                      |
| 53     | AI识别     | OpenSafety\_UDP              |
| 54     | AI识别     | Oracle\_TCP                  |
| 55     | AI识别     | Ovation                      |
| 56     | AI识别     | PCWORX                       |
| 57     | AI识别     | PHONENIX\_CONTACT            |
| 58     | AI识别     | PTPv1                        |
| 59     | AI识别     | PTPv2                        |
| 60     | AI识别     | Redlion\_Crimson3            |
| 61     | AI识别     | RSSP\_1                      |
| 62     | AI识别     | Siemens\_Profinet\_IO\_CM    |
| 63     | AI识别     | Siemens\_S7                  |
| 64     | AI识别     | Siemens\_S7Plus              |
| 65     | AI识别     | SinecH1                      |
| 66     | AI识别     | SIP                          |
| 67     | AI识别     | SMB                          |
| 68     | AI识别     | SNMPv1                       |
| 69     | AI识别     | SNMPv3                       |
| 70     | AI识别     | Supcon\_JX300                |
| 71     | AI识别     | TFTP                         |
| 72     | AI识别     | TLS\_HTTPs                   |
| 73     | AI识别     | Tridium\_Niagara\_Fox        |
| 74     | AI识别     | VNC\_UDP                     |
| 75     | AI识别     | Wago\_CoDeSys                |
| 76     | AI识别     | Yokogawa\_Vnet\_IP           |
| 77     | AI识别     | 安控\_sl304                    |
| 78     | AI识别     | 步科Kinco                      |
| 79     | AI识别     | 大工计控                         |
| 80     | AI识别     | 丹东华通\_2000R                  |
| 81     | AI识别     | 昆仑通态 MCGS                    |
| 82     | AI识别     | 力控实时数据库                      |
| 83     | AI识别     | 南大傲拓                         |
| 84     | AI识别     | 南大奥拓\_NA-RTU                 |
| 85     | AI识别     | 上海新华DCS TCP（XHICAN）          |
| 86     | AI识别     | 松下Panasonic                  |
| 87     | AI识别     | 上海新华DCS UDP                  |
| 88     | AI识别     | 研华Advantech                  |
| 89     | AI识别     | 中自DCS                        |
| 90     | AI识别     | Emerson\_Deltav              |
| 91     | AI识别     | GSK                          |
| 92     | AI识别     | HNC                          |
| 93     | AI识别     | MEMOBUS\_UDP                 |
| 94     | AI识别     | IPMI                         |
| 95     | AI识别     | Wonderware\_Service          |
| 96     | AI识别     | ShangHaiYangBang\_BX\_5E     |
| 97     | AI识别     | Wonderware\_Suitelink        |
| 98     | AI识别     | Wonderware\_NmxSvc\_tcp      |
| 99     | AI识别     | Wonderware\_NmxSvc\_udp      |
| 100    | AI识别     | HoneyWell\_tcp               |

> 端口识别：共计22种协议，协议范围如下

| **序号** | **识别方式** | **协议名称**               |
| ------ | -------- | ---------------------- |
| 1      | 端口识别     | ATG                    |
| 2      | 端口识别     | CSPv4\_2222            |
| 3      | 端口识别     | CSPv4\_6000            |
| 4      | 端口识别     | DNS\_UDP               |
| 5      | 端口识别     | Echo\_TCP              |
| 6      | 端口识别     | ENIP\_UDP              |
| 7      | 端口识别     | FF\_FMS                |
| 8      | 端口识别     | FF\_SM                 |
| 9      | 端口识别     | FTP                    |
| 10     | 端口识别     | Lantronix              |
| 11     | 端口识别     | LLMNR                  |
| 12     | 端口识别     | NetBios\_NS            |
| 13     | 端口识别     | NTP                    |
| 14     | 端口识别     | POP3                   |
| 15     | 端口识别     | PowerLink\_UDP         |
| 16     | 端口识别     | SMTP                   |
| 17     | 端口识别     | SSH                    |
| 18     | 端口识别     | Syslog\_WinServer2003  |
| 19     | 端口识别     | Telnet                 |
| 20     | 端口识别     | VxWorks\_Debug\_Reboot |
| 21     | 端口识别     | ZigBee\_UDP            |
| 22     | 端口识别     | 易控                     |

> 代码识别：共计18种协议，协议范围如下

| **序号** | **识别方式** | **协议名称**                |
| ------ | -------- | ----------------------- |
| 1      | 代码识别     | CDP                     |
| 2      | 代码识别     | EtherCAT\_L2            |
| 3      | 代码识别     | HoneyWell\_FTE          |
| 4      | 代码识别     | IEC61850-GOOSE协议        |
| 5      | 代码识别     | IEC61850-SMV协议          |
| 6      | 代码识别     | LLC                     |
| 7      | 代码识别     | LLDP                    |
| 8      | 代码识别     | OpenSafety\_SercosIII   |
| 9      | 代码识别     | PowerLink\_Layer2       |
| 10     | 代码识别     | SchneiderFoxboro\_IA    |
| 11     | 代码识别     | Siemens\_Profinet\_DCP  |
| 12     | 代码识别     | Siemens\_Profinet\_MRP  |
| 13     | 代码识别     | Siemens\_S5             |
| 14     | 代码识别     | Siemens\_Profinet\_PTCP |
| 15     | 代码识别     | TTE\_PCF                |
| 16     | 代码识别     | Siemens\_Profinet\_MRRT |
| 17     | 代码识别     | Siemens\_Profinet\_RTC3 |
| 18     | 代码识别     | Siemens\_Profinet\_RTC1 |

协议识别测试标准

> TCP/UDP消息无协议不识别、漏识别或误识别的情况，二层协议数据帧无协议不识别、漏识别或误识别的情况

测试用例说明

> AI识别：

Bacnet协议报文如下图所示

![](产品质量\_li\_img/media/image1.png)

ISTP Web显示结果如下图所示

![](产品质量\_li\_img/media/image2.png)

> 端口识别：

易控协议报文如下图所示

![](产品质量\_li\_img/media/image3.png)

ISTP Release显示结果如下图所示

![](产品质量\_li\_img/media/image4.png)

> 代码识别：

Siemens\_Profinet\_MRP协议报文如下图所示

![](产品质量\_li\_img/media/image5.png)

ISTP Web显示结果如下图所示

![](产品质量\_li\_img/media/image6.png)

### 1.2. 协议解析

#### 1.2.1. 功能说明

如果将工业设备比喻为人，那么工业协议就是指语言。不同的语言想要实现对话交流，就需要翻译，将传达的信息转化双方都能理解的一种形式，这就是协议解析。协议解析指的是面对不同协议的工业设备实现数据采集传输的能力，通过协议解析将设备连接起来并转换同一种协议，这样就能方便连接到更多的平台和设备，实现统一化的系统架构与集约化的生产。

ISTP支持49种协议的解析。

#### 1.2.2. 发布的标准

**1.2.2.1. MMS**

支持15种字段的解析，主要字段如下所示：

> mms\_pdu
>
> invoke\_id
>
> service
>
> variable\_access\_specification
>
> objects
>
> variable\_specification
>
> objectName
>
> domainId
>
> itemId
>
> vmd-specific
>
> aa-specific
>
> address
>
> symbolicAddress
>
> numericAddress
>
> unconstrainedAddress

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中服务为read的帧的情况如下图所示：

![](产品质量\_li\_img/media/image7.png)

> ISTP对报文中服务为read的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image8.png)

**1.2.2.2. BACNET**

支持28种字段的解析，主要字段如下所示：

> lpdu\_bvlc\_type
>
> lpdu\_bvlc\_func
>
> lpdu\_ip
>
> lpdu\_port
>
> npdu\_version
>
> npdu\_control
>
> npdu\_dnet
>
> npdu\_dlen
>
> npdu\_hop\_cnt
>
> apdu\_type
>
> apdu\_service\_choice
>
> lpdu\_bvlc\_time\_to\_live
>
> apdu\_max\_resp
>
> apdu\_max\_segs
>
> apdu\_seg\_resp\_acpt
>
> apdu\_invoke\_id
>
> lpdu\_bvlc\_result
>
> apdu\_service\_ack\_choice
>
> apdu\_error\_choice
>
> npdu\_snet
>
> npdu\_slen
>
> npdu\_sadr\_type
>
> npdu\_sadr
>
> apdu\_reason
>
> npdu\_dadr\_mstp\_arcnet
>
> npdu\_dadr\_type
>
> npdu\_sadr\_mstp\_arcnet
>
> npdu\_msg\_type

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为Original-Unicast-NPDU (0x0a)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image9.png)

> ISTP对报文中功能码为Original-Unicast-NPDU (0x0a)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image10.png)

**1.2.2.3. CoAp**

支持12种字段的解析，主要字段如下所示：

> version
>
> type
>
> code
>
> message\_id
>
> token\_length
>
> payload\_len
>
> options\_num
>
> option\_type
>
> delta
>
> uri\_len
>
> uri\_value
>
> token

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Code为Empty Message (0)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image11.png)

> ISTP对报文中Code为Empty Message (0)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image12.png)

**1.2.2.4. DNP3 TCP**

支持5种字段的解析，主要字段如下所示：

> destination
>
> source
>
> function\_code
>
> object\_obj
>
> object\_var

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为Read (0x01)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image13.png)

> ISTP对报文中功能码为Read (0x01)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image14.png)

**1.2.2.5. DNP3 UDP**

支持5种字段的解析，主要字段如下所示：

> destination
>
> source
>
> function\_code
>
> object\_obj
>
> object\_var

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为Read (0x01)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image15.png)

> 报文中功能码为Read (0x01)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image16.png)

**1.2.2.6. ENIP**

支持4种字段的解析，主要字段如下所示：

> encap\_cmd
>
> services
>
> service
>
> iclass

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Command为Send Unit Data (0x0070)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image17.png)

> ISTP对报文中Command为Send Unit Data (0x0070)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image18.png)

**1.2.2.7. CIP\_COMMON**

支持4种字段的解析，主要字段如下所示：

encap\_cmd

services

service

> iclass

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中服务字段为Get Attributes All (0x01)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image19.png)

> ISTP对报文中服务字段为Get Attributes All (0x01)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image20.png)

**1.2.2.8. CIP\_Logix5000**

支持6种字段的解析，主要字段如下所示：

encap\_cmd

services

service

pIOI\_len

pIOI

> iclass

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中服务为0x4c的情况如下图所示：

![](产品质量\_li\_img/media/image21.png)

> ISTP对报文中服务为0x4c的检测情况如下图所示：

![](产品质量\_li\_img/media/image22.png)

**1.2.2.9. CIP\_PCCC**

支持6种字段的解析，主要字段如下所示：

encap\_cmd

services

service

iclass

pccc\_cmd

> pccc\_fnc

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中服务为0x4b的情况如下图所示：

![](产品质量\_li\_img/media/image23.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image24.png)

**1.2.2.10. Etrol\_SL304\_TCP**

支持4种字段的解析，主要字段如下所示：

> dtype
>
> dgroup
>
> did
>
> len

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中dtype为0x01的帧的情况如下图所示：

![](产品质量\_li\_img/media/image25.png)

> ISTP对报文中dtype为0x01的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image26.png)

**1.2.2.11. Focas**

支持4种字段的解析，主要字段如下所示：

> dir
>
> function\_code
>
> send\_flag
>
> data\_len

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为1的帧的情况如下图所示：

![](产品质量\_li\_img/media/image27.png)

> ISTP对报文中功能码为1的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image28.png)

**1.2.2.12. GDW 3761**

支持11种字段的解析，主要字段如下所示：

protocol\_id

frame\_len

dir

prm

fcb\_acd

fcv

func\_code

afn\_code

term\_address

master\_address

type

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为9的帧的情况如下图所示：

![](产品质量\_li\_img/media/image29.png)

> ISTP对报文中功能码为9的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image30.png)

**1.2.2.13. GOOSE**

支持18种字段的解析，主要字段如下所示：

> d\_mac
>
> s\_mac
>
> APPID
>
> Length
>
> gocbRef
>
> timeAllowedtoLive
>
> datSet
>
> goID
>
> t
>
> stNum
>
> sqNum
>
> test
>
> confRev
>
> ndsCom
>
> numDatSetEntries
>
> allData
>
> boolean
>
> bit-string

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中APPID为 0x0001 (1)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image31.png)

> ISTP对报文中APPID为 0x0001 (1)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image32.png)

**1.2.2.14. HartIP\_TCP**

支持99种字段的解析，主要字段如下所示：

> version
>
> message\_type
>
> message\_id
>
> status
>
> sequence\_number
>
> message\_length
>
> host\_type
>
> inactivity\_close\_timer
>
> frame\_type
>
> long\_address
>
> command
>
> length
>
> checksum
>
> response\_code
>
> device\_status
>
> expansion\_code
>
> expanded\_device\_type
>
> minimum\_number\_of\_request\_preambles
>
> hart\_universal\_revision
>
> device\_revision
>
> device\_software\_revision
>
> hardware\_rev\_and\_physical\_signaling
>
> flags
>
> device\_id
>
> minimum\_number\_of\_response\_preambles
>
> maximum\_number\_of\_device\_variables
>
> configuration\_change\_counter
>
> extended\_device\_status
>
> manufacturer\_id
>
> private\_label
>
> device\_profile
>
> short\_address
>
> pv\_units
>
> pv
>
> pv\_loop\_current
>
> pv\_percent\_range
>
> sv\_units
>
> sv
>
> tv\_units
>
> tv
>
> qv\_units
>
> qv
>
> poll\_address
>
> loop\_current\_mode
>
> primary\_variable\_classification
>
> secondary\_variable\_classification
>
> tertiary\_variable\_classification
>
> quaternary\_variable\_classification
>
> slots
>
> slot0\_data\_timestamp
>
> device\_variable
>
> device\_variable\_classification
>
> units
>
> device\_variable\_value
>
> device\_variable\_status
>
> message
>
> tag
>
> descriptor
>
> day
>
> month
>
> year
>
> transducer\_serail\_number
>
> transducer\_limit\_min\_span\_units
>
> upper\_transducer\_limit
>
> lower\_transducer\_limit
>
> minimum\_span
>
> pv\_alarm\_selection\_code
>
> pv\_transfer\_function\_code
>
> pv\_upper\_and\_lower\_range\_values\_units
>
> pv\_upper\_range\_value
>
> pv\_lower\_range\_value
>
> pv\_damping\_value
>
> write\_protect\_code
>
> reserved
>
> pv\_analog\_channel\_flags
>
> final\_assembly\_number
>
> command\_number
>
> index\_of\_first\_discrete\_variable
>
> number\_of\_discrete\_variables
>
> timestamp\_for\_most\_recent\_discrete\_change
>
> discrete\_variable\_state
>
> discrete\_variable\_status
>
> device\_specific\_status
>
> device\_operating\_mode
>
> standardized\_status\_0
>
> standardized\_status\_1
>
> analog\_channel\_saturated
>
> standardized\_status\_2
>
> standardized\_status\_3
>
> analog\_channel\_fixed
>
> io\_card
>
> channel
>
> embedded\_command\_delimiter
>
> embedded\_command
>
> command\_byte\_count
>
> number\_of\_commands
>
> commands
>
> command\_numuber
>
> preambles

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Message Type为Publish (2)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image33.png)

> ISTP对报文中Message Type为Publish (2)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image34.png)

**1.2.2.15. HartIP\_UDP**

支持99种字段的解析，主要字段如下所示：

> version
>
> message\_type
>
> message\_id
>
> status
>
> sequence\_number
>
> message\_length
>
> host\_type
>
> inactivity\_close\_timer
>
> frame\_type
>
> long\_address
>
> command
>
> length
>
> checksum
>
> response\_code
>
> device\_status
>
> expansion\_code
>
> expanded\_device\_type
>
> minimum\_number\_of\_request\_preambles
>
> hart\_universal\_revision
>
> device\_revision
>
> device\_software\_revision
>
> hardware\_rev\_and\_physical\_signaling
>
> flags
>
> device\_id
>
> minimum\_number\_of\_response\_preambles
>
> maximum\_number\_of\_device\_variables
>
> configuration\_change\_counter
>
> extended\_device\_status
>
> manufacturer\_id
>
> private\_label
>
> device\_profile
>
> short\_address
>
> pv\_units
>
> pv
>
> pv\_loop\_current
>
> pv\_percent\_range
>
> sv\_units
>
> sv
>
> tv\_units
>
> tv
>
> qv\_units
>
> qv
>
> poll\_address
>
> loop\_current\_mode
>
> primary\_variable\_classification
>
> secondary\_variable\_classification
>
> tertiary\_variable\_classification
>
> quaternary\_variable\_classification
>
> slots
>
> slot0\_data\_timestamp
>
> device\_variable
>
> device\_variable\_classification
>
> units
>
> device\_variable\_value
>
> device\_variable\_status
>
> message
>
> tag
>
> descriptor
>
> day
>
> month
>
> year
>
> transducer\_serail\_number
>
> transducer\_limit\_min\_span\_units
>
> upper\_transducer\_limit
>
> lower\_transducer\_limit
>
> minimum\_span
>
> pv\_alarm\_selection\_code
>
> pv\_transfer\_function\_code
>
> pv\_upper\_and\_lower\_range\_values\_units
>
> pv\_upper\_range\_value
>
> pv\_lower\_range\_value
>
> pv\_damping\_value
>
> write\_protect\_code
>
> reserved
>
> pv\_analog\_channel\_flags
>
> final\_assembly\_number
>
> command\_number
>
> index\_of\_first\_discrete\_variable
>
> number\_of\_discrete\_variables
>
> timestamp\_for\_most\_recent\_discrete\_change
>
> discrete\_variable\_state
>
> discrete\_variable\_status
>
> device\_specific\_status
>
> device\_operating\_mode
>
> standardized\_status\_0
>
> standardized\_status\_1
>
> analog\_channel\_saturated
>
> standardized\_status\_2
>
> standardized\_status\_3
>
> analog\_channel\_fixed
>
> io\_card
>
> channel
>
> embedded\_command\_delimiter
>
> embedded\_command
>
> command\_byte\_count
>
> number\_of\_commands
>
> commands
>
> command\_numuber
>
> preambles

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Message Type为Publish (2)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image35.png)

> ISTP对报文中Message Type为Publish (2)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image36.png)

**1.2.2.16. HuaTong\_2000R\_TCP**

支持3种字段的解析，主要字段如下所示：

func\_code

addr

> data

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为5的帧的情况如下图所示：

![](产品质量\_li\_img/media/image37.png)

> ISTP对报文中功能码为5的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image38.png)

**1.2.2.17. IEC104**

支持17种字段的解析，主要字段如下所示：

> apdus
>
> apdu\_len
>
> frame\_type
>
> tx
>
> rx
>
> sq
>
> num\_ix
>
> test
>
> netgative
>
> cause\_tx
>
> oa
>
> type\_id
>
> addr
>
> IOA
>
> utype
>
> instrument\_type
>
> point\_table

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Type Id为141的帧的情况如下图所示：

![](产品质量\_li\_img/media/image39.png)

> ISTP对报文中Type Id为141的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image40.png)

**1.2.2.18. JX300**

支持2种字段的解析，主要字段如下所示：

> function\_code
>
> sequence

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image41.png)

> ISTP对报文中功能码为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image42.png)

**1.2.2.19. MELSEC\_TCP**

支持8种字段的解析，主要字段如下所示：

> data\_len
>
> wait\_time
>
> command
>
> sub\_command
>
> batch.unit
>
> batch.sc
>
> batch.range
>
> res\_code

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为1025的帧的情况如下图所示：

![](产品质量\_li\_img/media/image43.png)

> ISTP对报文中功能码为1025的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image44.png)

**1.2.2.20. Modbus\_TCP**

支持4种字段的解析，主要字段如下所示：

> function\_code
>
> address
>
> address\_length
>
> sub\_function\_code

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码分别为Read Coils和Diagnostics的帧的情况如下图所示：

![](产品质量\_li\_img/media/image45.png)

![](产品质量\_li\_img/media/image46.png)

> ISTP对报文中功能码分别为Read Coils和Diagnostics的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image47.png)

![](产品质量\_li\_img/media/image48.png)

**1.2.2.21. Modbus\_UDP**

支持4种字段的解析，主要字段如下所示：

> function\_code
>
> address
>
> address\_length
>
> sub\_function\_code

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码分别为Read Coils和Diagnostics的帧的情况如下图所示：

![](产品质量\_li\_img/media/image49.png)

![](产品质量\_li\_img/media/image50.png)

> ISTP对报文中功能码分别为Read Coils和Diagnostics的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image51.png)

![](产品质量\_li\_img/media/image52.png)

**1.2.2.22. Modbus\_UMAS**

支持3种字段的解析，主要字段如下所示：

> function\_code
>
> sub\_function\_code
>
> umas\_sub\_function\_code

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为90，子功能码为3的帧的情况如下图所示：

![](产品质量\_li\_img/media/image53.png)

> ISTP对报文中功能码为90，子功能码为3的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image54.png)

**1.2.2.23. Modbus\_RTU（不支持）**

支持3种字段的解析，主要字段如下所示：

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> Wireshark检测情况如下图所示：
>
> ISTP检测情况如下图所示：

**1.2.2.24. MQTT**

支持29种字段的解析，主要字段如下所示：

> message\_type
>
> message\_flag
>
> mqtt\_payload\_len
>
> protocol\_len
>
> protocol
>
> version
>
> c\_flag
>
> keepalive
>
> client\_id\_len
>
> client\_id
>
> will\_topic\_len
>
> will\_topic
>
> will\_message\_len
>
> will\_message
>
> username\_len
>
> username
>
> passwd\_len
>
> passwd
>
> reserved
>
> ret\_code
>
> topic\_len
>
> topic
>
> msg\_id
>
> message
>
> meassge
>
> mesage
>
> topic\_qos
>
> topics
>
> qos

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Message Type为Subscribe Request的帧的情况如下图所示：

![](产品质量\_li\_img/media/image55.png)

> ISTP对报文中Message Type为Subscribe Request的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image56.png)

**1.2.2.25. NA\_RTU\_TCP**

支持5种字段的解析，主要字段如下所示：

> func\_code
>
> length
>
> addr
>
> data\_count
>
> data

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为0x61的帧的情况如下图所示：

![](产品质量\_li\_img/media/image57.png)

> ISTP对报文中功能码为0x61的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image58.png)

**1.2.2.26. OMRON\_TCP**

支持117种字段的解析，主要字段如下所示：

> dir
>
> command\_code
>
> memory\_area\_code
>
> begin\_address
>
> num\_items
>
> response\_code
>
> data
>
> beginning\_address
>
> mul\_memory\_area
>
> mul\_memory\_area\_count
>
> memory\_area\_code\_source
>
> beginning\_address\_source
>
> memory\_area\_code\_dest
>
> begin\_address\_dest
>
> parameter\_area\_code
>
> beginning\_word
>
> num\_of\_word
>
> req\_clear\_data
>
> program\_num
>
> project\_code
>
> last\_word
>
> password
>
> num\_bytes
>
> clear\_code
>
> mode
>
> data\_type
>
> CPU Unit model
>
> CPU Unit internal system version
>
> For system use
>
> Area data
>
> unit address
>
> number\_of\_items
>
> units address
>
> model number
>
> status
>
> fatal error data
>
> non fatal error data
>
> message number
>
> fal/fals number
>
> error message
>
> parameter
>
> average\_cycle\_time
>
> max\_cycle\_time
>
> min\_cycle\_time
>
> Year
>
> Month
>
> Date
>
> Hour
>
> Minute
>
> Second
>
> Day
>
> MessageNo
>
> Error\_reset\_FALS\_No
>
> Beginning\_Record\_No
>
> No\_of\_Records
>
> MAX\_No\_of\_Stored\_Records
>
> No\_of\_Stored\_Records
>
> Error\_Logs
>
> Error\_Code1
>
> Error\_Code2
>
> disk\_num
>
> beginng\_file\_position
>
> num\_of\_files
>
> disk\_data
>
> file\_data
>
> filename
>
> file\_position
>
> data\_length
>
> file\_capacity
>
> para\_code
>
> Disk\_No
>
> Parameter\_Code
>
> Volume\_Label
>
> Src\_Disk\_No
>
> Src\_File\_Name
>
> Dst\_Disk\_No
>
> Dst\_File\_Name
>
> Old\_File\_Name
>
> New\_File\_Name
>
> File\_Name
>
> num\_of\_words
>
> Data\_Length
>
> num\_of\_bits
>
> set\_reset\_specification
>
> bit\_flag
>
> Message
>
> FALSNo
>
> ErrorMessage
>
> fixed
>
> intelligent\_id\_no
>
> first\_word
>
> read\_length
>
> no\_of\_link\_nodes
>
> data\_link\_status
>
> cio\_area\_first\_word
>
> kind\_of\_dm
>
> no\_of\_total\_words
>
> network\_member\_data
>
> communications\_cycle\_time
>
> current\_polling\_unit\_node\_number
>
> cyclic\_operation
>
> cyc\_lic\_transmission\_status
>
> cyclic\_nono-fatal\_errors
>
> cyclic\_error\_counters
>
> status\_flags
>
> number\_of\_receptions
>
> beginning\_block\_number
>
> number\_od\_blocks
>
> number\_of\_blocks\_remaining
>
> total\_number\_of\_blocks
>
> type
>
> control\_data
>
> block\_number
>
> number\_of\_units
>
> number\_od\_units
>
> name\_Data
>
> name\_data

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Command为Frame Send的帧的情况如下图所示：

![](产品质量\_li\_img/media/image59.png)

> ISTP对报文中Command为Frame Send的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image60.png)

**1.2.2.27. OMRON\_UDP**

支持118种字段的解析，主要字段如下所示：

> dir
>
> command\_code
>
> memory\_area\_code
>
> begin\_address
>
> num\_items
>
> response\_code
>
> data
>
> beginning\_address
>
> mul\_memory\_area
>
> mul\_memory\_area\_count
>
> memory\_area\_code\_source
>
> beginning\_address\_source
>
> memory\_area\_code\_dest
>
> begin\_address\_dest
>
> parameter\_area\_code
>
> beginning\_word
>
> num\_of\_word
>
> req\_clear\_data
>
> program\_num
>
> project\_code
>
> last\_word
>
> password
>
> num\_bytes
>
> clear\_code
>
> mode
>
> data\_type
>
> CPU Unit model
>
> CPU Unit internal system version
>
> For system use
>
> Area data
>
> pc status
>
> unit address
>
> number\_of\_items
>
> units address
>
> model number
>
> status
>
> fatal error data
>
> non fatal error data
>
> message number
>
> fal/fals number
>
> error message
>
> parameter
>
> average\_cycle\_time
>
> max\_cycle\_time
>
> min\_cycle\_time
>
> Year
>
> Month
>
> Date
>
> Hour
>
> Minute
>
> Second
>
> Day
>
> MessageNo
>
> Error\_reset\_FALS\_No
>
> Beginning\_Record\_No
>
> No\_of\_Records
>
> MAX\_No\_of\_Stored\_Records
>
> No\_of\_Stored\_Records
>
> Error\_Logs
>
> Error\_Code1
>
> Error\_Code2
>
> disk\_num
>
> beginng\_file\_position
>
> num\_of\_files
>
> disk\_data
>
> file\_data
>
> filename
>
> file\_position
>
> data\_length
>
> file\_capacity
>
> para\_code
>
> Disk\_No
>
> Parameter\_Code
>
> Volume\_Label
>
> Src\_Disk\_No
>
> Src\_File\_Name
>
> Dst\_Disk\_No
>
> Dst\_File\_Name
>
> Old\_File\_Name
>
> New\_File\_Name
>
> File\_Name
>
> num\_of\_words
>
> Data\_Length
>
> num\_of\_bits
>
> set\_reset\_specification
>
> bit\_flag
>
> Message
>
> FALSNo
>
> ErrorMessage
>
> fixed
>
> intelligent\_id\_no
>
> first\_word
>
> read\_length
>
> no\_of\_link\_nodes
>
> data\_link\_status
>
> cio\_area\_first\_word
>
> kind\_of\_dm
>
> no\_of\_total\_words
>
> network\_member\_data
>
> communications\_cycle\_time
>
> current\_polling\_unit\_node\_number
>
> cyclic\_operation
>
> cyc\_lic\_transmission\_status
>
> cyclic\_nono-fatal\_errors
>
> cyclic\_error\_counters
>
> status\_flags
>
> number\_of\_receptions
>
> beginning\_block\_number
>
> number\_od\_blocks
>
> number\_of\_blocks\_remaining
>
> total\_number\_of\_blocks
>
> type
>
> control\_data
>
> block\_number
>
> number\_of\_units
>
> number\_od\_units
>
> name\_Data
>
> name\_data

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Command为Frame Send的帧的情况如下图所示：

![](产品质量\_li\_img/media/image61.png)

> ISTP对报文中Command为Frame Send的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image62.png)

**1.2.2.28. OPC\_DA**

支持12种字段的解析，主要字段如下所示：

> apdus
>
> dir
>
> Version
>
> Version(minor)
>
> PacketType
>
> PacketFlags
>
> DataRepresentation
>
> FragLength
>
> AuthLength
>
> CallID
>
> opc\_interface
>
> opc\_function

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中opc\_interface为IOPCShutdown和opc\_function为ShutdownRequest的帧的情况如下图所示：

![](产品质量\_li\_img/media/image63.png)

> ISTP对报文中opc\_interface为IOPCShutdown和opc\_function为ShutdownRequest的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image64.png)

**1.2.2.29. OPC\_UA**

支持68种字段的解析，主要字段如下所示：

> Message Type
>
> Chunk Type
>
> Message Size
>
> Version
>
> Receive Buffer Size
>
> Send Buffer Size
>
> Max Message Size
>
> Max Chunk Count
>
> End Point Url
>
> ChunkType
>
> Status Code
>
> Reason
>
> Server Uri
>
> Secure Channel Id
>
> Security Token Id
>
> Security Sequence Number
>
> Security RequestId
>
> NodeId Info.EncodingMask
>
> NodeId Info.Namespace Index
>
> NodeId Info.Identifier Numric
>
> Security policy uri
>
> Sender Certificate
>
> Receiver Certificate Thumbprint
>
> Sequence number
>
> Request Id
>
> EncodingMask
>
> NameSpaceIndex
>
> Timestamp
>
> RequestHandle
>
> ReturnDiagnostics
>
> TimeoutHint
>
> ClientProtocolVersion
>
> SecurityTokenRequestType
>
> MessageSecurityMode
>
> RequestLifetime
>
> ServiceResult
>
> ServerProtocolVersion
>
> ChannelId
>
> TokenId
>
> CreateAt
>
> RevisedLifetime
>
> ServerNonce
>
> Identifier\_Numeric
>
> IdentifierNumeric
>
> ApplicationUri
>
> ProductUri
>
> Text
>
> ApplicationType
>
> ServerUri
>
> EndpointUrl
>
> SessionName
>
> ClientNonce
>
> ClientCertificate
>
> RequestedSessionTimeout
>
> MaxResponseMessageSize
>
> maxRequestMessageSize
>
> MaxAge
>
> TimestampsToReturn
>
> AttributeId
>
> Id
>
> Value
>
> ServerTimestamp
>
> ReleaseContinuePoint
>
> StatusCode
>
> SubscriptionId
>
> MoreNotification
>
> SequenceNumber
>
> PublishTime

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Message Type为HEL的帧的情况如下图所示：

![](产品质量\_li\_img/media/image65.png)

> ISTP对报文中Message Type为HEL的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image66.png)

**1.2.2.30. Ovation\_TCP**

支持3种字段的解析，主要字段如下所示：

> type
>
> func\_code
>
> len

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为2的帧的情况如下图所示：

![](产品质量\_li\_img/media/image67.png)

> ISTP对报文中功能码为2的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image68.png)

**1.2.2.31. Profinet\_DCP**

支持33种字段的解析，主要字段如下所示：

> frame\_id
>
> service\_id
>
> service\_type
>
> xid
>
> reserved
>
> data\_length
>
> blocks
>
> option
>
> suboption
>
> block\_length
>
> block\_info
>
> ip
>
> subnet
>
> gateway
>
> block\_error
>
> block\_qualifier
>
> response\_delay
>
> nameofstation
>
> dev\_options
>
> typeofstation
>
> vendor\_id
>
> device\_id
>
> device\_role
>
> mac
>
> device\_instance\_high
>
> device\_instance\_low
>
> oem\_vendor\_id
>
> oem\_device\_id
>
> option\_code
>
> dhcpparameterlength
>
> dhcpcontrolparameterdata
>
> signal\_value
>
> value

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中ServiceID为Get的帧的情况如下图所示：

![](产品质量\_li\_img/media/image69.png)

> ISTP对报文中ServiceID为Get的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image70.png)

**1.2.2.32. Profinet\_MRP**

支持21种字段的解析，主要字段如下所示：

> version
>
> mrps
>
> type
>
> length
>
> sequence\_id
>
> domain\_uuid
>
> prio
>
> sa
>
> port\_role
>
> ring\_state
>
> transition
>
> time\_stamp
>
> interval
>
> blocked
>
> manufacturer\_oui
>
> ed1\_type
>
> ed1\_manufacturer\_data
>
> sub\_type
>
> sub\_length
>
> other\_prio
>
> other\_sa

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中MRP\_TLVHeader.Type为MRP\_Common的帧的情况如下图所示：

![](产品质量\_li\_img/media/image71.png)

> ISTP对报文中MRP\_TLVHeader.Type为MRP\_Common的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image72.png)

**1.2.2.33. Profinet\_MRRT**

支持8种字段的解析，主要字段如下所示：

> blocks
>
> frame\_id
>
> version
>
> type
>
> length
>
> sequence\_id
>
> domain\_uuid
>
> sa

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Type为Common的帧的情况如下图所示：

![](产品质量\_li\_img/media/image73.png)

> ISTP对报文中Type为Common的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image74.png)

**1.2.2.34. Profinet\_PTCP**

支持33种字段的解析，主要字段如下所示：

> blocks
>
> frame\_id
>
> reserved\_1
>
> reserved\_2
>
> delay10ns
>
> delay1ns
>
> sequence\_id
>
> delay1ns\_byte
>
> type
>
> length
>
> t2timestamp
>
> port\_mac\_address
>
> oui
>
> subtype
>
> irdata\_uuid
>
> t2port\_rx\_delay
>
> t3port\_tx\_delay
>
> flags
>
> current\_utc\_offset
>
> delay1ns\_fup
>
> master\_source\_address
>
> subdomain\_uuid
>
> epoch\_number
>
> seconds
>
> nano\_seconds
>
> master\_priority1\_priority
>
> master\_priority1\_level
>
> master\_priority1\_reserved
>
> master\_priority1\_active
>
> master\_priority2
>
> clock\_class
>
> clock\_accuracy
>
> clock\_variance

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为Profinet PTCP协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image75.png)

> ISTP对报文中为Profinet PTCP协议帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image76.png)

**1.2.2.35. Profinet\_RTC1**

支持11种字段的解析，主要字段如下所示：

> frame\_id
>
> cycle\_counter
>
> ignore
>
> reserved\_2
>
> station\_problem\_indicator
>
> provider\_state
>
> reserved\_1
>
> data\_valid
>
> redundancy
>
> state
>
> transfer\_status

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为Profinet RTC1协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image77.png)

> ISTP对报文中为Profinet RTC1协议帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image78.png)

**1.2.2.36. Profinet\_RTC3（解析不正确）**

支持15种字段的解析，主要字段如下所示：

> frame\_id
>
> cycle\_counter
>
> ignore
>
> reserved\_2
>
> station\_problem\_indicator
>
> provider\_state
>
> reserved\_1
>
> data\_valid
>
> redundancy
>
> state
>
> transfer\_status
>
> sfcrc16
>
> sub\_frames
>
> position
>
> data\_length

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为Profinet RTC3协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image79.png)

> ISTP对报文中为Profinet RTC3协议帧的检测情况如下图所示：

**1.2.2.37. RSSP-1**

支持17种字段的解析，主要字段如下所示：

> interaction\_type
>
> protocol\_type
>
> src\_address
>
> dst\_address
>
> seq\_number
>
> data\_len
>
> svc\_1
>
> svc\_2
>
> data\_value
>
> crc\_16
>
> seqenq\_1
>
> seqenq\_2
>
> rsp\_id
>
> req\_id
>
> seq\_init\_1
>
> seq\_init\_2
>
> data\_verion

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为RSSP-1协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image80.png)

> ISTP对报文中为RSSP-1协议帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image81.png)

**1.2.2.38. S7**

支持113种字段的解析，主要字段如下所示：

> TpktVersion
>
> TpktReserved
>
> TpktLength
>
> CotpLength
>
> CotpPduType
>
> CotpTpduNumber
>
> CotpLastDataUnit
>
> ProtocolId
>
> ROSCTR
>
> RedundancyIndetification
>
> ProtocolDataUnitReference
>
> ParameterLength
>
> DataLength
>
> Items
>
> FunctionCode
>
> ErrorClass
>
> ErrorCode
>
> Address
>
> AddressLength
>
> SyntaxId
>
> VariableSpecification
>
> FollowingAddrLength
>
> DBNumber
>
> Area
>
> TransportSize
>
> FileName
>
> malformed\_error
>
> ParameterHead
>
> userdata\_ParameterLength
>
> Method
>
> Type
>
> FunctionGroup
>
> SubFunction
>
> SequenceNumber
>
> ReturnCode
>
> Length
>
> DataUnitReferenceNumber
>
> LastDataUnit
>
> TISParameterSize
>
> TISDataSize
>
> TISParameter
>
> ItemCount
>
> MemoryArea
>
> RepetitionFactor
>
> StartAddress
>
> IntervalTimeBase
>
> IntervalTimeFactor
>
> LengthofFollowingAddressSpecification
>
> Data
>
> Function
>
> JobId
>
> NumberofAreas
>
> SubItems
>
> BlockType
>
> BlockCount
>
> BlockNumber
>
> BlockFlags
>
> BlockLanguages
>
> FileSystem
>
> LengthofInfo
>
> BlockInfo2
>
> Constant3
>
> BytesBlockInfo
>
> BlockLanguage
>
> SubblkType
>
> LengthLoadMemory
>
> BlockSecurity
>
> CodeTimestamp
>
> InterfaceTimestamp
>
> SSBLength
>
> ADDLength
>
> LocalDataLength
>
> MC7CodeLength
>
> Author
>
> Family
>
> Name
>
> Version
>
> BlockCheckSum
>
> Reserved1
>
> Reserved2
>
> SZLId
>
> SZLIndex
>
> SZLPartialListLength
>
> SZLPartialListCount
>
> Index
>
> Key
>
> Param
>
> Real
>
> BartSch
>
> CrstWrst
>
> Res
>
> SubscribedEvents
>
> UserName
>
> Result
>
> EventId
>
> Priority
>
> OBNumber
>
> DatId
>
> AdditionalInformation1
>
> AdditionalInformation2
>
> TimeStampYear2
>
> TimeStampMonth
>
> TimeStampDay
>
> TimeStampHour
>
> TimeStampMinute
>
> TimeStampSecond
>
> TimeStampMilliSecond
>
> FunctionIdentifier
>
> NumberofMessageObjects
>
> QueryType
>
> TimeStampReserved
>
> TimeStampYear1
>
> TimeStampWeekday

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Function group为Programmer commands (1)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image82.png)

> ISTP对报文中Function group为Programmer commands (1)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image83.png)

**1.2.2.39. S7\_Plus**

支持24种字段的解析，主要字段如下所示：

> protid
>
> protoversion
>
> datalen
>
> opcode
>
> reserved1
>
> function\_code
>
> reserved2
>
> seqnum
>
> session\_id
>
> transport\_flag
>
> trailer\_protid
>
> trailer\_protoversion
>
> trailer\_datalen
>
> digestlen
>
> digest
>
> keepalive\_seqnum
>
> reserved
>
> keepalivesequencenumber
>
> subscrobjectid
>
> unknown2
>
> unknown3
>
> unknown4
>
> credittick
>
> subscrchgcnt

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Function为CreateObject (0x04ca)的帧的情况如下图所示：

![](产品质量\_li\_img/media/image84.png)

> ISTP对报文中Function为CreateObject (0x04ca)的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image85.png)

**1.2.2.40. GE\_SRTP**

支持7种字段的解析，主要字段如下所示：

> service\_request\_code
>
> segment\_selector
>
> data\_offset
>
> violate\_specs
>
> field\_name
>
> error\_code
>
> offset

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中服务请求码为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image86.png)

> ISTP对报文中服务请求码为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image87.png)

**1.2.2.41. SV**

支持15种字段的解析，主要字段如下所示：

> d\_mac
>
> s\_mac
>
> APPID
>
> Length
>
> Reserved 1
>
> Reserved 2
>
> noASDU
>
> ASDUs
>
> svID
>
> smpCnt
>
> confRef
>
> smpSynch
>
> seqData
>
> datSet
>
> smpRate

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为SV协议的帧的情况如下图所示：

![](产品质量\_li\_img/media/image88.png)

> ISTP对报文中为SV协议的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image89.png)

**1.2.2.42. Shanghaixinhua\_DCS**

支持5种字段的解析，主要字段如下所示：

> name
>
> len
>
> packtype
>
> unused
>
> cmd

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中命令为0x0900的帧的情况如下图所示：

![](产品质量\_li\_img/media/image90.png)

> ISTP对报文中命令为0x0900的帧的情况检测情况如下图所示：

![](产品质量\_li\_img/media/image91.png)

**1.2.2.43. IEC103\_UDP（NR）（解析不正确）**

支持14种字段的解析，主要字段如下所示：

> apdus
>
> FirstFlag
>
> Length
>
> SecondFlag
>
> SourceFactoryId
>
> SourceAddr
>
> DestinationFactoryId
>
> DestinationAddr
>
> DataNumber
>
> DeviceType
>
> DeviceState
>
> FirstRouterAddr
>
> LastRouterAddr
>
> Reserved

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为IEC103 UDP协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image92.png)

> ISTP对报文中为IEC103 UDP协议帧的检测情况如下图所示：

**1.2.2.44. DICOM**

支持59种字段的解析，主要字段如下所示：

> pdu\_type
>
> pdu\_len
>
> proto\_version
>
> called\_ae\_title
>
> calling\_ae\_title
>
> app\_item\_type
>
> app\_item\_len
>
> app\_item\_str
>
> present\_ctxs
>
> userinfo\_item\_type
>
> userinfo\_item\_len
>
> userinfo\_max\_item\_type
>
> userinfo\_max\_item\_len
>
> userinfo\_max\_pdu\_len
>
> userinfo\_uid\_item\_type
>
> userinfo\_uid\_item\_len
>
> userinfo\_uid
>
> userinfo\_async\_item\_type
>
> userinfo\_async\_item\_len
>
> userinfo\_async\_max\_num\_ops\_inv
>
> userinfo\_async\_max\_num\_ops\_per
>
> userinfo\_version\_item\_type
>
> userinfo\_version\_item\_len
>
> userinfo\_version
>
> present\_item\_type
>
> present\_item\_len
>
> present\_ctx\_id
>
> present\_result
>
> abstract\_item\_type
>
> abstract\_item\_len
>
> abstract\_item\_str
>
> transfer\_syns
>
> userinfo\_role\_sel\_item\_type
>
> userinfo\_role\_sel\_item\_len
>
> userinfo\_role\_sel\_sop\_class\_uid\_len
>
> userinfo\_role\_sel\_sopclassuid\_str
>
> userinfo\_role\_sel\_scu\_role
>
> userinfo\_role\_sel\_scp\_role
>
> userinfo\_extneg\_item\_type
>
> userinfo\_extneg\_item\_len
>
> userinfo\_extneg\_sop\_class\_uid\_len
>
> userinfo\_extneg\_sopclassuid\_str
>
> userinfo\_user\_idt\_item\_type
>
> userinfo\_user\_idt\_item\_len
>
> userinfo\_user\_idt\_type
>
> userinfo\_user\_idt\_resp\_req
>
> userinfo\_user\_idt\_primary\_field\_len
>
> userinfo\_user\_idt\_primary\_field\_str
>
> userinfo\_user\_idt\_secondary\_field\_len
>
> userinfo\_user\_idt\_secondary\_field\_str
>
> reject\_result
>
> reject\_source
>
> reject\_reason
>
> pdvs
>
> pdv\_len
>
> ctx\_id
>
> flags
>
> abort\_source
>
> abort\_reason

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为DICOM协议帧的情况如下图所示：

![](产品质量\_li\_img/media/image93.png)

> ISTP对报文中为DICOM协议帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image94.png)

**1.2.2.45. EtherCat**

支持14种字段的解析，主要字段如下所示：

> Length
>
> Reserved
>
> Type
>
> Datagrams\_num
>
> Attack\_flag
>
> Datagrams
>
> cmd
>
> index
>
> addr
>
> length
>
> round\_trip
>
> last\_indicator
>
> interrupt
>
> working\_cnt

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中Type为EtherCAT command (0x1)情况如下图所示：

![](产品质量\_li\_img/media/image95.png)

> ISTP对报文中Type为EtherCAT command (0x1)检测情况如下图所示：

![](产品质量\_li\_img/media/image96.png)

**1.2.2.46. GSK**

支持17种字段的解析，主要字段如下所示：

> unknown\_1
>
> local\_mac
>
> serpid\_1
>
> des\_mac
>
> serpid\_2
>
> pack\_no
>
> unknown\_8
>
> send\_to\_id
>
> data\_len
>
> unknown\_10
>
> next\_action
>
> file\_handle
>
> tran\_data\_len
>
> data\_size
>
> dir\_handle
>
> recv\_from\_id
>
> unknown\_12

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文为GSK的帧的情况如下图所示：

![](产品质量\_li\_img/media/image97.png)

> ISTP对报文为GSK的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image98.png)

**1.2.2.47. HL7**

支持80种字段的解析，主要字段如下所示：

> field\_separator
>
> component\_separator
>
> repetition\_separator
>
> escape\_character
>
> subcomponent\_separator
>
> message\_type
>
> trigger\_event
>
> segments
>
> field1
>
> field2
>
> field3
>
> field4
>
> field5
>
> field6
>
> field7
>
> field8
>
> field9
>
> field10
>
> field11
>
> field12
>
> field13
>
> field14
>
> field15
>
> field16
>
> field17
>
> field18
>
> field19
>
> field20
>
> field21
>
> field22
>
> field23
>
> field24
>
> field25
>
> field26
>
> field27
>
> field28
>
> field29
>
> field30
>
> field31
>
> field32
>
> field33
>
> field34
>
> field35
>
> field36
>
> field37
>
> field38
>
> field39
>
> field40
>
> field41
>
> field42
>
> field43
>
> field44
>
> field45
>
> field46
>
> field47
>
> field48
>
> field49
>
> field50
>
> field51
>
> field52
>
> field53
>
> field54
>
> field55
>
> field56
>
> field57
>
> field58
>
> field59
>
> field60
>
> field61
>
> field62
>
> field63
>
> field64
>
> field65
>
> field66
>
> field67
>
> field68
>
> field69
>
> field70
>
> field71
>
> field72

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中为HL7协议的帧的情况如下图所示：

![](产品质量\_li\_img/media/image99.png)

> ISTP对报文中为HL7协议的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image100.png)

**1.2.2.48. HNC**

支持8种字段的解析，主要字段如下所示：

> type
>
> source\_ip
>
> source\_port
>
> msg\_type
>
> msg\_flag
>
> msg\_length
>
> client\_no
>
> msg\_mask

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中message type为1的帧的情况如下图所示：

![](产品质量\_li\_img/media/image101.png)

> ISTP对报文中message type为1的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image102.png)

**1.2.2.49. HoneyWel**

支持12种字段的解析，主要字段如下所示：

> head\_seq\_no
>
> payload\_len
>
> seq\_no1
>
> seq\_no2
>
> body\_len
>
> item\_num
>
> items
>
> item\_seq\_no
>
> item\_len
>
> item\_type
>
> control
>
> func\_code

发布标准：

> 请求帧和响应帧均上报解析日志；
>
> 非畸形帧不漏报解析日志；

测试用例举例说明：

> 报文中功能码为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image103.png)

> ISTP对报文中功能码为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image104.png)

### 1.3. 协议白名单

#### 1.3.1. 功能说明

协议白名单是基于协议解析的基础上，将识别出的重要的协议字段作为白名单字段进行识别检测的功能。

支持49种协议的白名单检测。

#### 1.3.2. 发布的标准

**1.3.2.1. MMS**

支持10种字段的解析，主要字段如下所示：

> pdu\_type
>
> service
>
> object\_name
>
> arg1
>
> arg2
>
> arg2\_split\_0
>
> arg2\_split\_1
>
> arg2\_split\_2
>
> arg2\_split\_3
>
> address

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为write帧的情况如下图所示如下图：

![](产品质量\_li\_img/media/image105.png)

![](产品质量\_li\_img/media/image106.png)

> ISTP检测报文中功能码为write帧的情况如下图所示如下图：

![](产品质量\_li\_img/media/image107.png)

![](产品质量\_li\_img/media/image108.png)

**1.3.2.2. BACNET**

支持3种字段的解析，主要字段如下所示：

> white\_bvlc\_function
>
> white\_apdu\_type
>
> white\_apdu\_service

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为Forwarded-NPDU帧的情况如下图所示：

![](产品质量\_li\_img/media/image109.png)

> ISTP对报文中功能码为Forwarded-NPDU帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image110.png)

**1.3.2.3. CoAp**

支持4种字段的解析，主要字段如下所示：

> type
>
> code
>
> uri\_path.len
>
> uri\_path.value

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为GET的帧的情况如下图所示：

![](产品质量\_li\_img/media/image111.png)

> ISTP对报文中功能码为GET的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image112.png)

**1.3.2.4. DNP3 TCP**

支持5种字段的解析，主要字段如下所示：

> destination
>
> source
>
> function\_code
>
> object\_obj
>
> object\_var

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为Read的帧的情况如下图所示：

![](产品质量\_li\_img/media/image113.png)

> ISTP对报文中功能码为Read的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image114.png)

**1.3.2.5. DNP3 UDP**

支持5种字段的解析，主要字段如下所示：

> destination
>
> source
>
> function\_code
>
> object\_obj
>
> object\_var

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为write的帧的情况如下图所示：

![](产品质量\_li\_img/media/image115.png)

> ISTP对报文中功能码为write的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image116.png)

**1.3.2.6. ENIP**

支持1种字段的解析，主要字段如下所示：

> command

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为List Services的帧的情况如下图所示：

![](产品质量\_li\_img/media/image117.png)

> ISTP对报文中功能码为List Services的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image118.png)

**1.3.2.7. CIP\_COMMON**

支持2种字段的解析，主要字段如下所示：

> service
>
> iclass

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中服务为Get Attributes All的帧的情况如下图所示：

![](产品质量\_li\_img/media/image119.png)

> ISTP对报文中服务为Get Attributes All的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image120.png)

**1.3.2.8. CIP\_Logix5000**

支持4种字段的解析，主要字段如下所示：

> service
>
> iclass
>
> pIOI\_len
>
> pIOI

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中服务为Multiple Service Packet的帧的情况如下图所示：

![](产品质量\_li\_img/media/image121.png)

> ISTP对报文中服务为Multiple Service Packet的帧的情况如下图所示：

![](产品质量\_li\_img/media/image122.png)

**1.3.2.9. CIP\_PCCC**

支持4种字段的解析，主要字段如下所示：

> service
>
> iclass
>
> pccc\_fnc
>
> pccc\_cmd

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中服务为Execute PCCC的帧的情况如下图所示：

![](产品质量\_li\_img/media/image123.png)

> ISTP对报文中服务为Execute PCCC的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image124.png)

**1.3.2.10. Etrol\_SL304\_TCP**

支持3种字段的解析，主要字段如下所示：

> dtype
>
> dgroup
>
> did

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中dtype为0x01的帧的情况如下图所示：

![](产品质量\_li\_img/media/image125.png)

> ISTP对报文中dtype为0x01的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image126.png)

**1.3.2.11. Focas**

支持1种字段的解析，主要字段如下所示：

> function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为1的帧的情况如下图所示：

![](产品质量\_li\_img/media/image127.png)

> ISTP对报文中功能码为1的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image128.png)

**1.3.2.12. GDW 3761**

支持3种字段的解析，主要字段如下所示：

> afn\_code
>
> term\_address
>
> master\_address

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image129.png)

> ISTP对报文中功能码为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image130.png)

**1.3.2.13. GOOSE**

支持4种字段的解析，主要字段如下所示：

> appid
>
> gocbRef
>
> goid
>
> datSet

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> appid为001的帧的情况如下图所示：

![](产品质量\_li\_img/media/image131.png)

> ISTP对appid为001的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image132.png)

**1.3.2.14. HartIP\_TCP**

支持5种字段的解析，主要字段如下所示：

> message\_id
>
> frame\_type
>
> long\_address
>
> command
>
> short\_address

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Frame Type为2的帧的情况如下图所示：

![](产品质量\_li\_img/media/image133.png)

![](产品质量\_li\_img/media/image134.png)

> ISTP对报文中Frame Type为2的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image135.png)

![](产品质量\_li\_img/media/image136.png)

**1.3.2.15. HartIP\_UDP**

支持5种字段的解析，主要字段如下所示：

> message\_id
>
> frame\_type
>
> long\_address
>
> command
>
> short\_address

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Frame Type为2的帧的情况如下图所示：

![](产品质量\_li\_img/media/image137.png)

![](产品质量\_li\_img/media/image138.png)

> ISTP对报文中Frame Type为2的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image139.png)

![](产品质量\_li\_img/media/image140.png)

**1.3.2.16. HuaTong\_2000R\_TCP**

支持2种字段的解析，主要字段如下所示：

> func\_code
>
> addr

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 功能码为5的帧的情况如下图所示：

![](产品质量\_li\_img/media/image141.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image142.png)

**1.3.2.17. IEC104**

支持3种字段的解析，主要字段如下所示：

> type\_id
>
> addr
>
> IOA

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中TypeId为45的帧的情况如下图所示：

![](产品质量\_li\_img/media/image143.png)

> ISTP对报文中TypeId为45的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image144.png)

**1.3.2.18. JX300**

支持1种字段的解析，主要字段如下所示：

> function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image145.png)

> ISTP对报文中功能码为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image146.png)

**1.3.2.19. MELSEC\_TCP**

支持2种字段的解析，主要字段如下所示：

> command
>
> sub\_command

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为1025的帧的情况如下图所示：

![](产品质量\_li\_img/media/image147.png)

> ISTP对报文中功能码为1025的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image148.png)

**1.3.2.20. Modbus\_TCP**

支持4种字段的解析，主要字段如下所示：

> function\_code
>
> start\_addr
>
> end\_addr
>
> sub\_function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为1 的帧的情况如下图所示：

![](产品质量\_li\_img/media/image149.png)

> ISTP对报文中功能码为1 的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image150.png)

**1.3.2.21. Modbus\_UDP**

支持4种字段的解析，主要字段如下所示：

> function\_code
>
> start\_addr
>
> end\_addr
>
> sub\_function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为1 的帧的情况如下图所示：

![](产品质量\_li\_img/media/image151.png)

> ISTP对报文中功能码为1 的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image152.png)

**1.3.2.22. Modbus\_UMAS**

支持3种字段的解析，主要字段如下所示：

> function\_code
>
> sub\_function\_code
>
> umas\_sub\_function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为90 的帧的情况如下图所示：

![](产品质量\_li\_img/media/image153.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image154.png)

**1.3.2.23. Modbus\_RTU（不支持）**

支持3种字段的解析，主要字段如下所示：

> function\_code
>
> start\_addr
>
> end\_addr

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为1 的帧的情况如下图所示：

![](产品质量\_li\_img/media/image155.png)

> ISTP对报文中功能码为1 的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image156.png)

**1.3.2.24. MQTT**

支持7种字段的解析，主要字段如下所示：

> message\_type
>
> username\_len
>
> username
>
> passwd\_len
>
> passwd
>
> topic\_len
>
> topic

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Message Type分别为Connect Command和Public Message的帧的情况如下图所示：

![](产品质量\_li\_img/media/image157.png)

![](产品质量\_li\_img/media/image158.png)

> ISTP对报文中Message Type分别为Connect Command和Public Message的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image159.png)

![](产品质量\_li\_img/media/image160.png)

**1.3.2.25. NA\_RTU\_TCP**

支持2种字段的解析，主要字段如下所示：

> func\_code
>
> addr

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为0x61的帧的情况如下图所示：

![](产品质量\_li\_img/media/image161.png)

> ISTP对报文中功能码为0x61的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image162.png)

**1.3.2.26. OMRON\_TCP**

支持7种字段的解析，主要字段如下所示：

> command\_code
>
> arg1
>
> arg2
>
> arg3
>
> arg4
>
> arg5
>
> arg6

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码分别为0x0105 Memory Area Transfer和0x2202 Single File Read的帧的情况如下图所示：

![](产品质量\_li\_img/media/image163.png)

![](产品质量\_li\_img/media/image164.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image165.png)

![](产品质量\_li\_img/media/image166.png)

**1.3.2.27. OMRON\_UDP**

支持7种字段的解析，主要字段如下所示：

> command\_code
>
> arg1
>
> arg2
>
> arg3
>
> arg4
>
> arg5
>
> arg6

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码分别为0x0105 Memory Area Transfer和0x2202 Single File Read的帧的情况如下图所示：

![](产品质量\_li\_img/media/image167.png)

![](产品质量\_li\_img/media/image168.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image169.png)

![](产品质量\_li\_img/media/image170.png)

**1.3.2.28. OPC\_DA**

支持2种字段的解析，主要字段如下所示：

> opc\_interface
>
> opc\_function

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中opc\_interface为IOPCShutdown且opc\_function为ShutdownRequest情况如下图所示：

![](产品质量\_li\_img/media/image171.png)

> ISTP对报文中opc\_interface为IOPCShutdown且opc\_function为ShutdownRequest的检测情况如下图所示：

![](产品质量\_li\_img/media/image172.png)

**1.3.2.29. OPC\_UA**

支持3种字段的解析，主要字段如下所示：

> message\_type
>
> chunk\_type
>
> identifier\_numeric

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Message Type为MSG的帧的情况如下图所示：

![](产品质量\_li\_img/media/image173.png)

> ISTP对报文中Message Type为MSG的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image174.png)

**1.3.2.30. Ovation\_TCP**

支持2种字段的解析，主要字段如下所示：

> type
>
> func\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为2的帧的情况如下图所示：

![](产品质量\_li\_img/media/image175.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image176.png)

**1.3.2.31. Profinet\_DCP**

支持4种字段的解析，主要字段如下所示：

> service\_id
>
> service\_type
>
> option
>
> suboption

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为Set的帧的情况如下图所示：

![](产品质量\_li\_img/media/image177.png)

> ISTP对报文中功能码为Set的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image178.png)

**1.3.2.32. Profinet\_MRP**

支持4种字段的解析，主要字段如下所示：

> type
>
> arg1
>
> arg3
>
> arg2

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Type类型分别为MRP\_Common和MRP\_Option的帧的情况如下图所示：

![](产品质量\_li\_img/media/image179.png)

![](产品质量\_li\_img/media/image180.png)

> ISTP对报文中Type类型分别为MRP\_Common和MRP\_Option的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image181.png)

![](产品质量\_li\_img/media/image182.png)

**1.3.2.33. Profinet\_MRRT**

支持3种字段的解析，主要字段如下所示：

> type
>
> arg1
>
> arg2

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Type为0x01 Common的帧的情况如下图所示：

![](产品质量\_li\_img/media/image183.png)

> ISTP对报文中Type为0x01 Common的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image184.png)

**1.3.2.34. Profinet\_PTCP**

支持5种字段的解析，主要字段如下所示：

> type
>
> arg3
>
> arg4
>
> arg1
>
> arg2

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Type分别为1和2的帧的情况如下图所示：

![](产品质量\_li\_img/media/image185.png)

![](产品质量\_li\_img/media/image186.png)

> ISTP对报文中Type分别为1和2的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image187.png)

![](产品质量\_li\_img/media/image188.png)

**1.3.2.35. Profinet\_RTC1**

支持1种字段的解析，主要字段如下所示：

> frame\_id

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中FrameID为0x8000的帧的情况如下图所示：

![](产品质量\_li\_img/media/image189.png)

> ISTP对报文中FrameID为0x8000的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image190.png)

**1.3.2.36. Profinet\_RTC3**

支持1种字段的解析，主要字段如下所示：

> frame\_id

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中FrameID为0x0100的帧的情况如下图所示：

![](产品质量\_li\_img/media/image191.png)

> ISTP对报文中FrameID为0x0100的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image192.png)

**1.3.2.37. RSSP-1**

支持3种字段的解析，主要字段如下所示：

> interaction\_type
>
> src\_address
>
> dst\_address

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Interaction Type为0x01的帧的情况如下图所示：

![](产品质量\_li\_img/media/image193.png)

> ISTP检测情况如下图所示：

![](产品质量\_li\_img/media/image194.png)

**1.3.2.38. S7**

支持8种字段的解析，主要字段如下所示：

> FunctionCode
>
> Area
>
> StartAddr
>
> DBNumber
>
> TransportSize
>
> EndAddr
>
> FunctionGroup
>
> SubFunction

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中分别为功能码为Read Var以及功能码组为Cyclic Services的帧的情况如下图所示：

![](产品质量\_li\_img/media/image195.png)

![](产品质量\_li\_img/media/image196.png)

> ISTP对报文中分别为功能码为Read Var以及功能码组为Cyclic Services的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image197.png)

![](产品质量\_li\_img/media/image198.png)

**1.3.2.39. S7\_Plus**

支持2种字段的解析，主要字段如下所示：

> opcode
>
> function\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为Explore的帧的情况如下图所示：

![](产品质量\_li\_img/media/image199.png)

> ISTP对报文中功能码为Explore的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image200.png)

**1.3.2.40. GE\_SRTP**

支持3种字段的解析，主要字段如下所示：

> service\_request\_code
>
> segment\_selector
>
> data\_offset

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Service Request Code为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image201.png)

> ISTP对报文中Service Request Code为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image202.png)

**1.3.2.41. SV**

支持2种字段的解析，主要字段如下所示：

> appid
>
> svid

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中APPID为0x4000的帧的情况如下图所示：

![](产品质量\_li\_img/media/image203.png)

> ISTP对报文中APPID为0x4000的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image204.png)

**1.3.2.42. Shanghaixinhua\_DCS**

支持5种字段的解析，主要字段如下所示：

> name
>
> len
>
> packtype
>
> unused
>
> cmd

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中命令为0x0900的帧的情况如下图所示：

![](产品质量\_li\_img/media/image90.png)

> ISTP对报文中命令为0x0900的帧的情况检测情况如下图所示：

![](产品质量\_li\_img/media/image205.png)

**1.3.2.43. IEC103\_UDP（NR）**

支持4种字段的解析，主要字段如下所示：

> SourceFactoryId
>
> SourceAddr
>
> DestinationFactoryId
>
> DestinationAddr

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中SourceFactoryId、DestinationFactoryId都为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image206.png)

> ISTP对报文中SourceFactoryId、DestinationFactoryId都为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image207.png)

**1.3.2.44. DICOM**

支持1种字段的解析，主要字段如下所示：

> pdu\_type

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中PDU Type为ASSOC Request的帧的情况如下图所示：

![](产品质量\_li\_img/media/image208.png)

> ISTP对报文中PDU Type为ASSOC Request的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image209.png)

**1.3.2.45. EtherCat**

支持4种字段的解析，主要字段如下所示：

> Type
>
> Datagrams
>
> cmd
>
> index

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Type为0的帧的情况如下图所示：

![](产品质量\_li\_img/media/image210.png)

> ISTP对报文中Type为0的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image211.png)

**1.3.2.46. GSK**

支持3种字段的解析，主要字段如下所示：

> send\_to\_id
>
> local\_mac
>
> des\_mac

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Send To Id为0x01的帧的情况如下图所示：

![](产品质量\_li\_img/media/image212.png)

> ISTP对报文中Send To Id为0x01的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image213.png)

**1.3.2.47. HL7**

支持2种字段的解析，主要字段如下所示：

> message\_type
>
> trigger\_event

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中Message Type为RDE的帧的情况如下图所示：

![](产品质量\_li\_img/media/image214.png)

> ISTP对报文中Message Type为RDE的帧的检测情况如下图所示：

![](产品质量\_li\_img/media/image215.png)

**1.3.2.48. HNC**

支持2种字段的解析，主要字段如下所示：

> type
>
> msg\_type

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> Wireshark检测情况如下图所示：
>
> ISTP检测情况如下图所示：

**1.3.2.49. HoneWell**

支持5种字段的解析，主要字段如下所示：

> item\_num
>
> items
>
> item\_type
>
> control
>
> func\_code

发布标准：

> 响应帧不上报白名单日志；
>
> 非畸形请求帧不漏报白名单日志；

测试用例举例说明：

> 报文中功能码为0的情况如下图所示：

![](产品质量\_li\_img/media/image216.png)

> ISTP对报文中功能码为0的检测情况如下图所示：

![](产品质量\_li\_img/media/image217.png)

### 1.4. 关键事件检测

#### 1.4.1. 功能说明

通过对流量中的关键操作指令（如启动、停止、上传、下载等）进行解析及检测；从而实现对协议关键操作的检测。目前，ISTP支持31种协议的关键事件检测。

#### 1.4.2. 发布的标准

**1.4.2.1. MMS**

该协议支持如下52种关键事件

| **关键事件ID** | **关键事件名称** |
| ---------- | ---------- |
| 1          | 重命名        |
| 2          | 写          |
| 3          | 定义有名变量     |
| 4          | 定义离散访问     |
| 5          | 删除变量访问     |
| 6          | 定义有名变量列表   |
| 7          | 删除有名变量列表   |
| 8          | 定义有名类型     |
| 9          | 删除有名类型     |
| 10         | 输入         |
| 11         | 输出         |
| 12         | 取得控制       |
| 13         | 放弃控制       |
| 14         | 定义信号量      |
| 15         | 删除信号量      |
| 16         | 初始下载序列     |
| 17         | 下载段        |
| 18         | 结束下载序列     |
| 19         | 初始上载序列     |
| 20         | 上载段        |
| 21         | 结束上载序列     |
| 22         | 请求域下载      |
| 23         | 请求域上载      |
| 24         | 装载域内容      |
| 25         | 存储域内容      |
| 26         | 删除域        |
| 27         | 创建程序调用     |
| 28         | 删除程序调用     |
| 29         | 开始         |
| 30         | 停止         |
| 31         | 继续         |
| 32         | 复位         |
| 33         | 截杀         |
| 34         | 获得文件       |
| 35         | 定义事件条件     |
| 36         | 删除事件条件     |
| 37         | 调整事件条件监视   |
| 38         | 触发事件       |
| 39         | 定义事件动作     |
| 40         | 删除事件动作     |
| 41         | 定义事件入口     |
| 42         | 删除事件入口     |
| 43         | 调整事件入口     |
| 44         | 写日志        |
| 45         | 初始日志       |
| 46         | 创建日志       |
| 47         | 删除日志       |
| 48         | 文件重命名      |
| 49         | 文件删除       |
| 50         | 文件打开       |
| 51         | 文件读        |
| 52         | 文件关闭       |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以MMS协议“文件打开”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image218.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。
>
> <img src="产品质量_li_img/media/image219.png" alt="" data-size="original">

**1.4.2.2. BACNET**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称                  |
| ------ | ----------------------- |
| 2      | 注册外部设备                  |
| 3      | 从表中删除外部设备               |
| 4      | 外部设备可以使BBMD在所有IP子网上广播消息 |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“注册外部设备”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image220.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。
>
> <img src="产品质量_li_img/media/image221.png" alt="" data-size="original">

**1.4.2.3. CoAp**

该协议支持如下15种关键事件

| 关键事件ID | 关键事件名称                 |
| ------ | ---------------------- |
| 1      | Bad Request            |
| 2      | Unauthorized           |
| 3      | Bad Option             |
| 4      | Forbidden              |
| 5      | Not Found              |
| 6      | Method Not Allowed     |
| 7      | Not Acceptable         |
| 8      | Precondition Failed    |
| 9      | Unsuppor Conten-Type   |
| 10     | Internal Server Error  |
| 11     | Not Implemented        |
| 12     | Bad Gateway            |
| 13     | Service Unavailable    |
| 14     | Gateway Timeout        |
| 15     | Proxying Not Supported |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“Method Not Allowed”关键事件为例，报文内容如下图所示。

![](产品质量\_li\_img/media/image222.png)

> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image223.png)

**1.4.2.4. DNP3**

该协议支持如下16种关键事件

| 关键事件ID | 关键事件名称   |
| ------ | -------- |
| 2      | 冷再启动     |
| 3      | 暖再启动     |
| 4      | 保存配置     |
| 5      | 删除文件     |
| 6      | 恢复出厂设置   |
| 7      | 初始化应用程序  |
| 8      | 启动应用程序   |
| 9      | 停止应用程序   |
| 10     | 打开文件     |
| 11     | 关闭文件     |
| 12     | 获取文件信息   |
| 13     | 文件认证     |
| 14     | 文件传输中止   |
| 15     | 身份认证请求   |
| 16     | 身份认证失败通知 |
| 17     | 身份认证响应   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“冷再启动”关键事件为例，报文内容如下图所示。

![](产品质量\_li\_img/media/image224.png)

> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image225.png)

**1.4.2.5. CIP\_COMMON**

该协议支持如下12种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 3      | 复位     |
| 4      | 启动     |
| 5      | 停止     |
| 6      | 创建     |
| 7      | 删除     |
| 8      | 应用属性   |
| 10     | 恢复     |
| 11     | 保存     |
| 13     | 插入成员   |
| 14     | 移除成员   |
| 15     | 下装     |
| 16     | 上载     |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“复位”关键事件为例，报文内容如下图所示。

![](产品质量\_li\_img/media/image226.png)

> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image227.png)

**1.4.2.6. CIP\_PCCC**

该协议支持如下22种关键事件

| 关键事件ID | 关键事件名称                      |
| ------ | --------------------------- |
| 20     | download all request        |
| 21     | download completed          |
| 22     | download request            |
| 23     | file write                  |
| 29     | restart request             |
| 30     | set CPU mode                |
| 31     | shutdown                    |
| 35     | upload all request (upload) |
| 36     | upload completed            |
| 37     | upload                      |
| 40     | open file                   |
| 41     | change mode                 |
| 42     | close file                  |
| 43     | disable forces              |
| 44     | disable outputs             |
| 45     | enable outputs              |
| 46     | enable PLC scanning         |
| 47     | enter download mode         |
| 48     | enter upload mode           |
| 49     | exit download/upload mode   |
| 50     | file read                   |
| 51     | initialize memory           |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“download all request”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image228.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image229.png)

**1.4.2.7. Etrol\_SL304\_TCP**

该协议支持如下6种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 井口配置   |
| 2      | RTU配置  |
| 3      | 开机     |
| 4      | 关机     |
| 5      | 读写ai量程 |
| 6      | 仪表告警   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“井口配置”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image230.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image231.png)

**1.4.2.8. Focas**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称            |
| ------ | ----------------- |
| 1      | SETUP\_CONNECTION |
| 2      | START             |
| 3      | STOP              |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“START”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image232.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image233.png)

**1.4.2.9. GDW 3761**

该协议支持如下2种关键事件

| 关键事件ID | 关键事件名称    |
| ------ | --------- |
| 1      | 复位        |
| 2      | 身份认证及密钥协商 |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“ 复位”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image234.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image235.png)

**1.4.2.10. GOOSE**

该协议支持如下1种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 检修状态   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“检修状态”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image236.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image237.png)

**1.4.2.11. HartIP**

该协议支持如下5种关键事件

| 关键事件ID | 关键事件名称        |
| ------ | ------------- |
| 1      | 设置轮询地址        |
| 2      | 写短标签、设备描述符和日期 |
| 3      | 写最终装配号        |
| 4      | 写长标签          |
| 5      | 复位配置改变标志      |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“复位配置改变标志”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image238.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image239.png)

**1.4.2.12. HuaTong\_2000R\_TCP**

该协议支持如下9种关键事件

| 关键事件ID | 关键事件名称   |
| ------ | -------- |
| 1      | 油井启动     |
| 2      | 油井停止     |
| 3      | 加热炉燃烧器点火 |
| 4      | 加热炉燃烧器关断 |
| 5      | 电动抱闸抱死   |
| 6      | 电动抱闸松开   |
| 7      | 平衡调节启动   |
| 8      | 平衡调节停止   |
| 9      | RTU复位    |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“油井启动”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image240.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image241.png)

**1.4.2.13. IEC104**

该协议支持如下13种关键事件

| 关键事件ID | 关键事件名称            |
| ------ | ----------------- |
| 1      | 单命令               |
| 2      | 带时间标签的单命令         |
| 3      | 双命令               |
| 4      | 带时间标签的双命令         |
| 5      | 调节step命令          |
| 6      | 带时间标签的调节step命令    |
| 8      | 设置浮点命令，带时间标签的规范值  |
| 9      | 设置浮点命令，换算值        |
| 10     | 设置浮点命令，带时间标签的换算值  |
| 11     | 设置浮点命令，短浮点数       |
| 12     | 设置浮点命令，带时间标签的短浮点数 |
| 13     | 32位bitstring      |
| 15     | 重置进程命令            |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“单命令”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image242.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image243.png)

**1.4.2.14. JX300**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 发送设备信息 |
| 2      | 设置设备值  |
| 3      | 设置设备状态 |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“发送设备信息”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image244.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image245.png)

**1.4.2.15. MELSEC**

该协议支持如下19种关键事件

| 关键事件ID | 关键事件名称     |
| ------ | ---------- |
| 1      | 远程运行       |
| 2      | 远程停止       |
| 3      | 远程暂停       |
| 4      | 远程锁存清除     |
| 5      | 远程重置       |
| 6      | 远程锁        |
| 7      | 远程解锁       |
| 8      | 错误信息清除     |
| 9      | 新建文件       |
| 10     | 删除文件       |
| 11     | 复制文件       |
| 12     | 文件属性修改     |
| 13     | 文件创建时间修改   |
| 14     | 打开文件       |
| 15     | 读文件        |
| 16     | 写文件        |
| 17     | 关闭文件       |
| 18     | 写缓冲存储器     |
| 19     | 写智能模块缓冲存储器 |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“远程运行”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image246.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image247.png)

**1.4.2.16. Modbus**

该协议支持如16种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 写单线圈   |
| 2      | 写多线圈   |
| 3      | 写单寄存器  |
| 4      | 写多寄存器  |
| 5      | PLC启动  |
| 6      | PLC停止  |
| 7      | 开始下装   |
| 8      | 结束下装   |
| 9      | 开始上传   |
| 10     | 结束上传   |
| 11     | 强制置1   |
| 12     | 强制置0   |
| 13     | 强制取消   |
| 15     | 掩码写寄存器 |
| 16     | 读写寄存器  |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“PLC启动”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image248.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。
>
> <img src="产品质量_li_img/media/image249.png" alt="" data-size="original">

**1.4.2.17. NA\_RTU\_TCP**

该协议支持如下10种关键事件

| 关键事件ID | 关键事件名称     |
| ------ | ---------- |
| 1      | 复位         |
| 2      | 关闭进程       |
| 3      | 关闭看门狗      |
| 4      | RTU参数配置-下载 |
| 5      | 仪表参数配置-设置  |
| 6      | 开井         |
| 7      | 关井         |
| 8      | 加热炉点火      |
| 9      | 加热炉熄火      |
| 10     | 设置油井频率     |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“复位”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image250.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image251.png)

**1.4.2.18. OMRON\_TCP**

该协议支持如下23种关键事件

| 关键事件ID | 关键事件名称                          |
| ------ | ------------------------------- |
| 1      | PLC\_RESET                      |
| 2      | PLC\_RUN                        |
| 3      | PLC\_STOP                       |
| 4      | FORCED\_SET\_RESET              |
| 5      | CLOCK\_WRITE                    |
| 7      | ACCESS\_RIGTH\_ACQUIRE          |
| 9      | PLC\_SINGLE\_FILE\_WRITE        |
| 10     | FORCED\_SET\_RESET\_CANCEL      |
| 11     | PLC\_ERROR\_CLEAR               |
| 12     | PLC\_ERROR\_LOG\_CLEAR          |
| 13     | ACCESS\_RIGHT\_FORCED\_ACQUIRE  |
| 14     | FILE\_DELETE                    |
| 16     | MEMORY\_FILL                    |
| 18     | PROGRAM\_CLEAR                  |
| 19     | PARAMETER\_PROTECT\_CLEAR       |
| 20     | PARAMETER\_AREA\_CLEAR          |
| 21     | PROGRAM\_AREA\_PROTECT          |
| 22     | MESSAGE\_CLEAR                  |
| 23     | FILE\_COPY                      |
| 24     | FILE\_NAME\_CHANGE              |
| 25     | MEMORY\_AREA\_FILE\_TRANSFER    |
| 26     | PARAMETER\_AREA\_FILE\_TRANSFER |
| 27     | PROGRAM\_AREA\_FILE\_TRANSFER   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“ ”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image252.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image253.png)

**1.4.2.19. OMRON\_UDP**

该协议支持如下23种关键事件

| 关键事件ID | 关键事件名称                          |
| ------ | ------------------------------- |
| 1      | PLC\_RESET                      |
| 2      | PLC\_RUN                        |
| 3      | PLC\_STOP                       |
| 4      | FORCED\_SET\_RESET              |
| 5      | CLOCK\_WRITE                    |
| 7      | ACCESS\_RIGTH\_ACQUIRE          |
| 9      | PLC\_SINGLE\_FILE\_WRITE        |
| 10     | FORCED\_SET\_RESET\_CANCEL      |
| 11     | PLC\_ERROR\_CLEAR               |
| 12     | PLC\_ERROR\_LOG\_CLEAR          |
| 13     | ACCESS\_RIGHT\_FORCED\_ACQUIRE  |
| 14     | FILE\_DELETE                    |
| 16     | MEMORY\_FILL                    |
| 18     | PROGRAM\_CLEAR                  |
| 19     | PARAMETER\_PROTECT\_CLEAR       |
| 20     | PARAMETER\_AREA\_CLEAR          |
| 21     | PROGRAM\_AREA\_PROTECT          |
| 22     | MESSAGE\_CLEAR                  |
| 23     | FILE\_COPY                      |
| 24     | FILE\_NAME\_CHANGE              |
| 25     | MEMORY\_AREA\_FILE\_TRANSFER    |
| 26     | PARAMETER\_AREA\_FILE\_TRANSFER |
| 27     | PROGRAM\_AREA\_FILE\_TRANSFER   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“ ”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image254.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image255.png)

**1.4.2.20. OPC\_UA**

该协议支持如下30种关键事件

| 关键事件ID | 关键事件名称         |
| ------ | -------------- |
| 1      | 服务错误请求         |
| 2      | 注册服务器请求        |
| 3      | 关闭安全通道请求       |
| 4      | 创建会话请求         |
| 5      | 激活会话请求         |
| 6      | 关闭会话请求         |
| 7      | 取消请求           |
| 8      | 添加节点请求         |
| 9      | 添加参考请求         |
| 10     | 删除节点请求         |
| 11     | 删除参考请求         |
| 12     | 将浏览路径转换为节点id请求 |
| 13     | 注册节点请求         |
| 14     | 注销节点请求         |
| 15     | 写请求            |
| 16     | 历史更新请求         |
| 17     | 调用请求           |
| 18     | 创建监视项请求        |
| 19     | 修改监视项请求        |
| 20     | 设置监视模式请求       |
| 21     | 设置触发请求         |
| 22     | 删除监视项请求        |
| 23     | 创建订阅请求         |
| 24     | 修改订阅请求         |
| 25     | 设置发布模式请求       |
| 26     | 发布请求           |
| 27     | 重新发布请求         |
| 28     | 订阅传输请求         |
| 29     | 订阅删除请求         |
| 30     | 测试堆栈请求         |
| 　      | 　              |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“激活会话请求”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image256.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image257.png)

**1.4.2.21. ovation\_tcp**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称        |
| ------ | ------------- |
| 1      | TCP\_RESTART  |
| 2      | TCP\_DOWNLOAD |
| 3      | TCP\_LOAD     |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“TCP\_RESTART”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image258.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image259.png)

![](产品质量\_li\_img/media/image260.png)

**1.4.2.22. Profinet\_DCP**

该协议支持如下1种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 设置请求   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“设置请求”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image261.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image262.png)

**1.4.2.23. Profinet\_MRP**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 4      | 拓扑更改操作 |
| 5      | 链路关闭   |
| 6      | 链路启动   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“链路关闭”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image263.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image264.png)

**1.4.2.24. Profinet\_MRRT**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | END    |
| 2      | COMMON |
| 3      | TEST   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“END”关键事件为例，报文内容如下图所示。

![](产品质量\_li\_img/media/image265.png)

> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image266.png)

**1.4.2.25. Profinet\_PTCP**

该协议支持如下9种关键事件

| 关键事件ID | 关键事件名称           |
| ------ | ---------------- |
| 1      | END              |
| 2      | SUBDOMAIN        |
| 3      | TIME             |
| 4      | TIME\_EXTENSION  |
| 5      | MASTER           |
| 6      | PORT\_PARAMETER  |
| 7      | DELAY\_PARAMETER |
| 8      | PORT\_TIME       |
| 9      | OPTION           |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“END”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image267.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。
>
> <img src="产品质量_li_img/media/image268.png" alt="" data-size="original">

**1.4.2.26. RSSP-1**

该协议支持如下1种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 时序校正请求 |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“时序校正请求”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image269.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image270.png)

**1.4.2.27. S7**

该协议支持如下24种关键事件

| 关键事件ID | 关键事件名称         |
| ------ | -------------- |
| 1      | 强制DI/AI        |
| 2      | 删除DI值          |
| 5      | 诊断             |
| 6      | 清空PLC内存        |
| 7      | 设置时钟           |
| 8      | 设置PLC密码        |
| 9      | 请求下载           |
| 10     | 开始下载           |
| 11     | 下载完成           |
| 13     | 开始上载           |
| 14     | 上载             |
| 15     | 上载结束           |
| 16     | PLC启动          |
| 17     | PLC停止          |
| 18     | 激活设备上下载的块      |
| 19     | 从设备的文件系统中删除一个块 |
| 20     | 压缩PLC内存        |
| 21     | 将RAM复制到ROM     |
| 23     | 暖启动            |
| 24     | 请求更新固件         |
| 25     | 更新固件           |
| 26     | 结束更新固件         |
| 27     | 停止             |
| 28     | 暖重启            |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“PLC启动”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image271.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image272.png)

**1.4.2.28. S7\_Plus**

该协议支持如下6种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 开始下装   |
| 2      | 下装结束   |
| 3      | 开始上传   |
| 5      | PLC启动  |
| 6      | PLC停止  |
| 7      | 系统时间   |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“PLC启动”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image273.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image274.png)

**1.4.2.29. GE\_SRTP**

该协议支持如下3种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 停止PLC  |
| 2      | 启动PLC  |
| 3      | 下载     |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“停止PLC”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image275.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image276.png)

**1.4.2.30. Shanghaixinhua\_DCS**

该协议支持如下4种关键事件

| 关键事件ID | 关键事件名称 |
| ------ | ------ |
| 1      | 上装     |
| 2      | 改密码    |
| 3      | 清空组态   |
| 4      | 复位控制器  |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“上装”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image277.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image278.png)

**1.4.2.31. HoneyWell**

该协议支持如下4种关键事件

| 关键事件ID | 关键事件名称             |
| ------ | ------------------ |
| 1      | IDLE               |
| 2      | COLDSTART          |
| 3      | WARMSTART          |
| 4      | MODE\_CAS          |
| 5      | MODE\_MAN          |
| 6      | MODE\_NOMAL        |
| 7      | EXEC\_STATUS\_IDLE |
| 8      | EXEC\_STATUS\_RUN  |
| 9      | OUTPUT\_ON         |
| 10     | OUTPUT\_OFF        |

发布标准

> 支持范围内的关键操作可上报关键事件，不漏报，不误报
>
> 报文中存在关键事件的数据帧，上报相应关键事件
>
> 响应帧不上报关键事件

测试用例举例说明

> 以该协议“WARMSTART”关键事件为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image279.png" alt="" data-size="original">
>
> ISTP检测结果，如下图所示。

![](产品质量\_li\_img/media/image280.png)

![](产品质量\_li\_img/media/image281.png)

### 1.5. 畸形和规约检测

#### 1.5.1. 功能说明

针对工控协议中相关字段进行语义语法检查，如果字段存在格式错误，数据帧无法正常解析，则上报畸形告警日志；如果字段存在语义错误，数据帧可以正常解析，上报规约告警日志。目前支持39种工业协议的畸形和规约检测

#### 1.5.2. 发布的标准

**1.5.2.1. MMS**

支持97个字段的畸形和规约检测，具体字段如下所示：

TPKT\_version

TPKT\_len

COTP\_len

ISO8327\_SPDU

ISO8327\_len

ISO8823\_len

ISO8650\_len

MMS

MMS-PDU

invokeID

confirmedService

confirmedServiceRequest：rename

extendedObjectClass

ObjectClass

currentName

newIdentifier

specificationWithResult

variableAccessSpecificatn

listOfVariable

listOfVariable\_Variable

variableListName

VariableSpecification\_address

VariableSpecification\_name

variableDescription

scatteredAccessDescription

scatteredAccessDescription\_variableSpecification

Address\_numericAddress

Address\_symbolicAddress

Address\_unconstrainedAddress

TypeSpecification\_typeName

TypeSpecification\_array

TypeSpecification\_array\_packed

TypeSpecification\_array\_numberOfElements

TypeSpecification\_array\_elementType

TypeSpecification\_structure

TypeSpecification\_structure\_packed

TypeSpecification\_structure\_components

TypeSpecification\_structure\_components\_componentType

Response-variableAccessSpecificatn

Response-listOfAccessResult

Response-AccessResult\_failure

Response-Data\_array

Response-Data\_structure

Response-Data\_boolean

Response-Data\_BitString

Response-Data\_integer

Response-Data\_unsigned

Response-Data\_FloatingPoint

Response-Data\_octet\_string

Response-Data\_visiblestring

Response-Data\_binarytime

Response-Data\_bcd

Response-Data\_booleanArray

variableAccessSpecificatn\_listOfVariable

listOfData

Response-failure

Response-success

name

address

Response-mmsDeletable

Response-typeSpecification

DefineNamedVariableList

ObjectName\_vmd-specific

ObjectName\_domain-specific

ObjectName\_domain-specific\_domainId

ObjectName\_domain-specific\_itemId

ObjectName\_aa-specific

Response-listOfVariable

Response-listOfVariable\_Variable

scopeOfDelete

listOfVariableListName

Response\_numberMatched

Response\_numberDeleted

semaphoreName

namedToken

priority

acceptableDelay

controlTimeOut

abortOnTimeOut

relinquishIfConnectionLost

applicationToPreemptt

ResponsePDU-noResult

ResponsePDU-namedToken

Response-Data\_objId

Response-Data\_mMSString

Response-Data\_utc-time

PresentationCPType

PresentationCPTypeCXT

PresentationModeValue

PresentationModeParameter

acse\_len

acse\_cxt\_tag

presentation\_user\_data

presentation\_pdv\_list

presentation-context-identifier

presentation\_data\_values

padding

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

invokeID字段：在PDU支持范围内，按照对应规范解析失败，数据帧无法解析，上报畸形告警日志

ObjectName\_domain-specific\_domainId字段：在DefineNamedVariableList支持范围内，按照对应规范解析失败，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> mms协议invokeID tag非法，mms报文内容显示如下图所示
>
> <img src="产品质量_li_img/media/image282.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image283.png" alt="" data-size="original">

规约检查日志

> mms协议domainId非法，mms报文内容显示如下
>
> <img src="产品质量_li_img/media/image284.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image285.png" alt="" data-size="original">

**1.5.2.2. BACnet**

支持43个字段的畸形和规约检测，具体字段如下所示：

BVLC Type

BVLC Function

BVLC Length

BVLC-Result

Write-Broadcast-Distribution-Table

Read-Broadcast-Distribution-Table

Read-Broadcast-Distribution-Table-Ack

Forwarded-NPDU

Register-Foreign-Device

Read-Foreign-Device-Table

Read-Foreign-Device-Table-Ack

Delete-Foreign-Device-Table-Entry

Distribute-Broadcast-To-Network

Original-Unicast-NPDU

Original-Broadcast-NPDU

Version

Control

DNET

DLEN

DADR

SNET

SLEN

SADR

Hop Count

Message Type

Vendor ID

APDU

Type

segmented-message

max-segments-accepted

max-APDU-length-accepted

Invoke ID

sequence-number

proposed-window-size

service-choice

Reserve

actual-window-size

Reject Reason

Abort Reason

Error Service

ConfirmedRequestService

ServcerService

confirmedServiceAck

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

BVLC Type字段：BVLC Type不为0X81时，数据帧无法解析，上报畸形告警日志

Version字段：Version不为0X01时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> BACnet协议BVLC Type非法，BACnet报文显示如下
>
> <img src="产品质量_li_img/media/image286.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image287.png" alt="" data-size="original">

规约检查日志

> BACnet协议Version非法，BACnet报文显示如下
>
> <img src="产品质量_li_img/media/image288.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image289.png" alt="" data-size="original">

**1.5.2.3. DNP3**

支持14个字段的畸形和规约检测，具体字段如下所示：

Start Bytes

Data Link Header checksum

Data Link Layer Length

Data Link Layer Control Function Code

Data Chunk checksum

Application Layer Function Code

Object&\&Variant

reserved bit

Index Size

Qualifier Code

payload\_data

application\_layer

incorret\_string\_length\_data

incorret\_size\_data

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Start Bytes字段：首个Start非05，第二个Start非64时，数据帧无法解析，上报畸形告警日志

Data Link Layer Control Function Code字段：当PRM为1时，dl\_func有效取值为0x00, 0x01, 0x02, 0x03, 0x04, 0x09；当PRM为0时，dl\_func有效取值为0x00, 0x01, 0x0B。当该字段不在上述范围内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> DNP3协议Start Bytes非法，DNP3报文显示如下
>
> <img src="产品质量_li_img/media/image290.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image291.png" alt="" data-size="original">

规约检查日志

> DNP3协议Data Link Layer Control Function Code非法，DNP3报文显示如下
>
> <img src="产品质量_li_img/media/image292.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image293.png" alt="" data-size="original">

**1.5.2.4. ENIP\_CIP**

支持24个字段的畸形和规约检测，具体字段如下所示：

Command

Length

ltem Count

ENIP/CIP

Interface Handle

Address TypeID

Address length

Data Type ID

Data length

Service

Class

Request\_Path\_Size

CMD

FNC

Requestor ID Length

Request\_Path

Data Size

ANSI Symbol

Number of Services

Offsets

Size of Additional Status

Attribute Count

Reserved

name\_of\_service

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Size of Additional Status字段：Size of Additional Status长度与实际长度不一致时，数据帧无法解析，上报畸形告警日志

Class字段：Class未在范围值时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> ENIP\_CIP协议Size of Additional Status设置错误，ENIP\_CIP报文显示如下
>
> <img src="产品质量_li_img/media/image294.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image295.png" alt="" data-size="original">

规约检查日志

> ENIP\_CIP协议Class非法，ENIP\_CIP报文显示如下
>
> <img src="产品质量_li_img/media/image296.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image297.png" alt="" data-size="original">

**1.5.2.5. Goose**

支持25个字段的畸形和规约检测，具体字段如下所示：

Goose-APPID

Goose-Length

Goose-APDU

Goose-gocbReft

Goose-timeAllowedtoLivet

Goose-Datset

Goose-GoID

Goose-t

Goose-stNumt

Goose-sqNumt

Goose-test

Goose-confRev

Goose-ndsCom

Goose-numDatSetEntries

Goose-GOOSE

Goose-Pos.stVal

Goose-Pos.q

Goose-Pos.t

Goose-allData

Goose-numDatSetEntries

bit\_string\_length

utc-time

boolean

floating-point

binary-time

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Goose-timeAllowedtoLivet字段：tag不等于0x81；Length长度大于5或Length长度与实际长度不一致，数据帧无法解析，上报畸形包日志

Goose-APPID字段：Goose-APPID字段不在规范值0x0000\~0x3fff内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Goose协议timeAllowedtoLivet非法，Goose报文显示如下
>
> <img src="产品质量_li_img/media/image298.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image299.png" alt="" data-size="original">

规约检查日志

> Goose协议APPID非法，Goose报文显示如下
>
> <img src="产品质量_li_img/media/image300.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image301.png" alt="" data-size="original">

**1.5.2.6. IEC104**

支持15个字段的畸形和规约检测，具体字段如下所示：

Apdulen

TypeId

NumIx

CauseTx

MS

Min

Hour

Day

Month

control\_field3

control\_field2

control\_field4

Addr

IOA

SCO

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Addr字段：Addr字段缺失时，数据帧无法解析，上报畸形告警日志

CauseTx字段：CauseTx字段的值未在规范内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> IEC104协议Addr字段缺失，IEC104报文显示如下
>
> <img src="产品质量_li_img/media/image302.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image303.png" alt="" data-size="original">

规约检查日志

> IEC104协议CauseTx非法，IEC104报文显示如下
>
> <img src="产品质量_li_img/media/image304.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image305.png" alt="" data-size="original">

**1.5.2.7. Modbus**

支持43个字段的畸形和规约检测，具体字段如下所示：

Address

Quantity of coils(Bit\_Count)

Byte count

Coils status

Exception\_Code

Quantity of Inputs(Bit\_Count)

Inputs status

Quantity of Registe(Word\_Count)

Quantity of Input Registers(Word\_Count)

Input registers

Output value(Data)

Register value

Output date

Data

Sub-function

Event Count

Status

Quantity of Outputs(Bit\_Count)

Output value

Quantity of registers(Bit\_Count)

Registers value

Run indicator status

Sub-req.x,File Number

Sub-req.x,Record Number

Request data length

Reference address

and\_mask

or\_Mask

Quantity to read

Quantity to write

Write byte count

Read/Write registers value

FIFO count

FIFO value register

MEI type

payload\_error

Modbus\_length\_error

Protocol\_Identifier

function\_code

Reference Type

File Resp. length

Record Length

Object Value

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Address字段：Address字段缺失时，数据帧无法解析，上报畸形告警日志

Protocol\_Identifier字段：Protocol\_Identifier字段不为0x0000时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Modbus协议Address字段缺失，Modbus报文显示如下
>
> <img src="产品质量_li_img/media/image306.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image307.png" alt="" data-size="original">

规约检查日志

> Modbus协议Protocol\_Identifier非法，Modbus报文显示如下
>
> <img src="产品质量_li_img/media/image308.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image309.png" alt="" data-size="original">

**1.5.2.8. Modbus\_UDP**

支持43个字段的畸形和规约检测，具体字段如下所示：

Address

Quantity of coils(Bit\_Count)

Byte count

Coils status

Exception\_Code

Quantity of Inputs(Bit\_Count)

Inputs status

Quantity of Registe(Word\_Count)

Quantity of Input Registers(Word\_Count)

Input registers

Output value(Data)

Register value

Output date

Data

Sub-function

Event Count

Status

Quantity of Outputs(Bit\_Count)

Output value

Quantity of registers(Bit\_Count)

Registers value

Run indicator status

Sub-req.x,File Number

Sub-req.x,Record Number

Request data length

Reference address

and\_mask

or\_Mask

Quantity to read

Quantity to write

Write byte count

Read/Write registers value

FIFO count

FIFO value register

MEI type

payload\_error

Modbus\_length\_error

Protocol\_Identifier

function\_code

Reference Type

File Resp. length

Record Length

Object Value

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Address字段：Address字段缺失时，数据帧无法解析，上报畸形告警日志

Protocol\_Identifier字段：Protocol\_Identifier字段不为0x0000时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Modbus UDP协议Address字段缺失，Modbus UDP报文显示如下
>
> <img src="产品质量_li_img/media/image310.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image311.png" alt="" data-size="original">

规约检查日志

> Modbus UDP协议Protocol\_Identifier非法，Modbus UDP报文显示如下
>
> <img src="产品质量_li_img/media/image312.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image313.png" alt="" data-size="original">

**1.5.2.9. Omron\_TCP**

支持32个字段的畸形和规约检测，具体字段如下所示：

ICF

RSV (reserved)

GCT (Gateway Count)

DNA (Destination Network Address)

DA1 (Destination Node Address)

DA2 (Destination Units Address)

SNA (Source Network Address)

SA1 (Source Node Address)

SA2 (Source Units Address)

SID (Service ID)

OmronFins Command

OmronFins Response（End Code）

program No

No. of bytes

end code

Clear Code

Mode

Data

Unit Address

number of items

Error Message

parameter

Disk No

Beginning file postion

No.of files

Directory length

Parameter code

Set/reset designation

I/O memory area code

Bit/flag

Memory area code

BeginingWord

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

OmronFins Command字段：OmronFins Command字段不为有效功能码时，数据帧无法解析，上报畸形告警日志

ICF字段：ICF字段有效值为第8位为1，第2到6位为0，当ICF字段值与有效值不一致时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Omron\_tcp协议Command非法，Omron\_tcp报文显示如下
>
> <img src="产品质量_li_img/media/image314.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image315.png" alt="" data-size="original">

规约检查日志

> Omron\_tcp协议ICF非法，Omron\_tcp报文显示如下
>
> <img src="产品质量_li_img/media/image316.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image317.png" alt="" data-size="original">

**1.5.2.10. Omron\_UDP**

支持32个字段的畸形和规约检测，具体字段如下所示：

ICF

RSV (reserved)

GCT (Gateway Count)

DNA (Destination Network Address)

DA1 (Destination Node Address)

DA2 (Destination Units Address)

SNA (Source Network Address)

SA1 (Source Node Address)

SA2 (Source Units Address)

SID (Service ID)

OmronFins Command

OmronFins Response（End Code）

program No

No. of bytes

end code

Clear Code

Mode

Data

Unit Address

number of items

Error Message

parameter

Disk No

Beginning file postion

No.of files

Directory length

Parameter code

Set/reset designation

I/O memory area code

Bit/flag

Memory area code

BeginingWord

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

OmronFins Command字段：OmronFins Command字段不为有效功能码时，数据帧无法解析，上报畸形告警日志

ICF字段：ICF字段有效值为第8位为1，第2到6位为0，当ICF字段值与有效值不一致时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Omron\_tcp协议Command非法，Omron\_udp报文显示如下
>
> <img src="产品质量_li_img/media/image318.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image319.png" alt="" data-size="original">

规约检查日志

> Omron\_tcp协议ICF非法，Omron\_udp报文显示如下
>
> <img src="产品质量_li_img/media/image320.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image321.png" alt="" data-size="original">

**1.5.2.11. OPC DA**

支持12个字段的畸形和规约检测，具体字段如下所示：

Packet Flags

Data Representation的Byte order

Data Representation的Character

Data Representation的Floating-point

frag length

Auth length

StringBinding

UUID

OPNum

pdu\_type

context\_id

stringbinding\_NetwordAddr

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

UUID字段：UUID字段为非法值时，数据帧无法解析，上报畸形告警日志

Character字段：Data Representation的Character的值不为0时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> OPCDA协议UUID非法，OPCDA报文显示如下
>
> <img src="产品质量_li_img/media/image322.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image323.png" alt="" data-size="original">

规约检查日志

> OPCDA协议Data Representation的Character不为0，OPCDA报文显示如下
>
> <img src="产品质量_li_img/media/image324.png" alt="" data-size="original">
>
> 回放的OPCDA协议报文，ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image325.png" alt="" data-size="original">

**1.5.2.12. OPC UA**

支持23个字段的畸形和规约检测，具体字段如下所示：

Message Type

Reserved/isFinal

MessageSize

ProtocolVersion

ReceiveBufferSize

SendBufferSize

MaxMessageSize

MaxChunkCount

EndpointUrl

Error

Reason

ServerUri

SecureChannelId

SecurityPolicyUriLength

SecurityPolicyUri

SenderCertificateLength

SenderCertificate

ReceiverCertificateThumbprintLength

ReceiverCertificateThumbprint

TokenId

SequenceNumber

RequestId

encodingMask

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Message Type字段：Message Type字段不为 “HEL”、“ACK“、”ERR“、”RHE“、”OPN“、”CLO“、”MSG“时，数据帧无法解析，上报畸形告警日志

Reserved/isFinal字段：Reserved/isFinal字段不为值 “F”、“C“、”A“时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> OPCUA协议Message Type不在范围内，OPCUA报文显示如下
>
> <img src="产品质量_li_img/media/image326.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image327.png" alt="" data-size="original">

规约检查日志

> OPCUA协议Reserved/isFinal不在范围内，OPCUA报文显示如下
>
> <img src="产品质量_li_img/media/image328.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image329.png" alt="" data-size="original">

**1.5.2.13. S7**

支持38个字段的畸形和规约检测，具体字段如下所示：

TPKTVersion

TPKTLength

COTPLength

ROSCTR

Parameter Length

Data length

Error Class

Function

Item Count

Length of following address specification

Syntax Id

Transport size

Data中Transport size

DB Number

Area

Address

Parameter Item 与Data Item的数量

Retrun code

Parameter Item

PduLength

FilenameLength

File identifier

Block type

Block number

Destination filesystem

Length part 2

Mc7CodeLength

ErrorCode

Blocklengthstring Length

parameter block length

Number of blocks

blocktype

BlockNumber

DestFileSys

String length

PI Service

Part2StringLength

PiService

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

ROSCTR字段：ROSCTR字段不为值1、2、3、7时，数据帧无法解析，上报畸形告警日志

Error Class字段：Error Class字段不为值0x00、0x81-0x85、0x87时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> S7协议ROSCTR不在范围内，S7报文显示如下
>
> <img src="产品质量_li_img/media/image330.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image331.png" alt="" data-size="original">

规约检查日志

> S7协议Error Class不在范围内，S7报文显示如下
>
> <img src="产品质量_li_img/media/image332.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image333.png" alt="" data-size="original">

**1.5.2.14. SV**

支持15个字段的畸形和规约检测，具体字段如下所示：

SV-APPID

SV-length

SV-savPdu

SV-savPdu-noASDU

SV-savPdu-seqASDU

SV-savPdu-seqASDU-ASDU

SV-savPdu-seqASDU-SVID

SV-savPdu-seqASDU-DatSet

SV-savPdu-seqASDU-SmpCnt

SV-savPdu-seqASDU-ConfRev

SV-savPdu-seqASDU-RefrTm

SV-savPdu-seqASDU-smpSynch

SV-savPdu-seqASDU-SmpRate

SV-savPdu-seqASDU-seqData

sv

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

SV-savPdu-seqASDU-ASDU字段：ASDU的tag不为0x30或length与实际长度不一致，数据帧无法解析，上报畸形告警日志

SV-APPID字段：SV-APPID字段不为0x4000-0x7fff时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> SV协议SV-savPdu-seqASDU-ASDU非法，SV报文显示如下
>
> <img src="产品质量_li_img/media/image334.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image335.png" alt="" data-size="original">

规约检查日志

> SV协议SV-APPID非法，SV报文显示如下
>
> <img src="产品质量_li_img/media/image336.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image337.png" alt="" data-size="original">

**1.5.2.15. Coap**

支持2个字段的畸形和规约检测，具体字段如下所示：

version

code

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Version字段：Version字段值不为0x01时，数据帧无法解析，上报畸形告警日志

Code字段：Code字段不为值0、2、4、5时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Coap协议version非法，Coap报文显示如下
>
> <img src="产品质量_li_img/media/image338.png" alt="" data-size="original">
>
> 回放的Coap协议报文，ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image339.png" alt="" data-size="original">

规约检查日志

> Coap协议code非法，Coap报文显示如下
>
> <img src="产品质量_li_img/media/image340.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image341.png" alt="" data-size="original">

**1.5.2.16. DICOM**

支持5个字段的畸形和规约检测，具体字段如下所示：

pdu\_type

pdu\_len

pdv\_len

result

Item Type

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

pdu\_type字段：pdu\_type字段取值不是1，2，3，4，5，6，7时，数据帧无法解析，上报畸形告警日志

result字段：presentation中的result字段取值不为0，1，2，3，4时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> DICOM协议pdu\_type取值不在范围内，DICOM报文显示如下
>
> <img src="产品质量_li_img/media/image342.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image343.png" alt="" data-size="original">

规约检查日志

> DICOM协议presentation中的result取值不在范围内，DICOM报文显示如下
>
> <img src="产品质量_li_img/media/image344.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image345.png" alt="" data-size="original">

**1.5.2.17. EtherCat**

支持1个字段的规约检测，具体字段如下所示：

cmd

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

cmd字段：cmd字段值取值不在0x00-0x0E范围内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> EtherCat协议cmd不在范围内，EtherCat报文显示如下
>
> <img src="产品质量_li_img/media/image346.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image347.png" alt="" data-size="original">

**1.5.2.18. Etrol**

支持4个字段的畸形和规约检测，具体字段如下所示：

preamble

protocol

code

dtype

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

protocol字段：protocol字段缺失时，数据帧无法解析，上报畸形告警日志

preamble字段：preamble字段不为0x0189时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Etrol协议protocol字段缺失，Etrol报文显示如下
>
> <img src="产品质量_li_img/media/image348.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image349.png" alt="" data-size="original">

规约检查日志

> Etrol协议preamble不为0x0189，Etrol报文显示如下
>
> <img src="产品质量_li_img/media/image350.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image351.png" alt="" data-size="original">

**1.5.2.19. Focas**

支持4个字段的规约检测，具体字段如下所示：

FLAG1

FLAG2

Fun code

Req flag

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

FLAG1字段：FLAG1字段不为0xa0a0a0a0时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> Focas协议FLAG1不为0xa0a0a0a0，Focas报文显示如下
>
> <img src="产品质量_li_img/media/image352.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image353.png" alt="" data-size="original">

**1.5.2.20. GDW 376.1**

支持3个字段的畸形检测，具体字段如下所示：

start\_field

protocol id

Length

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

start\_field字段：start\_field字段不为0x68时，数据帧无法解析，上报畸形告警日志

测试用例举例说明

畸形检查日志

> GDW 376.1 协议start\_field不为0x68，GDW 376.1报文显示如下
>
> <img src="产品质量_li_img/media/image354.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image355.png" alt="" data-size="original">

**1.5.2.21. GE-SRTP**

支持3个字段的规约检测，具体字段如下所示：

message\_type

service\_request\_code

segment\_selector

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

service\_request\_code字段：service\_request\_code字段值取值未在协议规范范围内，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> GE-SRTP协议service\_request\_code字段值取值未在协议规范范围内，GE-SRTP报文显示如下
>
> <img src="产品质量_li_img/media/image356.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image357.png" alt="" data-size="original">

**1.5.2.22. GSK（error code错误导致后面两个字段没有值）**

支持2个字段的畸形检测，具体字段如下所示：

send\_to\_id

recv\_from\_id

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

send\_to\_id字段：send\_to\_id字段缺失时，数据帧无法解析，上报畸形告警日志

测试用例举例说明

畸形检查日志

> GSK协议send\_to\_id字段缺失，GSK报文显示如下
>
> <img src="产品质量_li_img/media/image358.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image359.png" alt="" data-size="original">

**1.5.2.23. HartIP\_TCP**

支持4个字段的畸形和规约检测，具体字段如下所示：

Message Type

Message ID

Frame Type

Byte Count

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Byte Count字段：Byte Count字段实际剩余长度减1 小于 length长度，数据帧无法解析，上报畸形告警日志

Message Type字段：Message Type字段值未在范围(0，1，2，3，15)内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> HartIP\_TCP协议Byte Count实际剩余长度错误，HartIP\_TCP报文显示如下
>
> <img src="产品质量_li_img/media/image360.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image361.png" alt="" data-size="original">

规约检查日志

> HartIP\_TCP协议Message Type不在预定范围内，HartIP\_TCP报文显示如下
>
> <img src="产品质量_li_img/media/image362.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image363.png" alt="" data-size="original">

**1.5.2.24. HartIP\_UDP**

支持4个字段的畸形和规约检测，具体字段如下所示：

Message Type

Message ID

Frame Type

Byte Count

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Byte Count字段：Byte Count字段实际剩余长度减1 小于 length长度，数据帧无法解析，上报畸形告警日志

Message Type字段：Message Type字段值未在范围(0，1，2，3，15)内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> HartIP\_UDP协议Byte Count实际剩余长度错误，HartIP\_UDP报文显示如下
>
> <img src="产品质量_li_img/media/image364.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image365.png" alt="" data-size="original">

规约检查日志

> HartIP\_UDP协议Message Type不在预定范围内，HartIP\_UDP报文显示如下
>
> <img src="产品质量_li_img/media/image366.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image367.png" alt="" data-size="original">

**1.5.2.25. HL7**

支持14个字段的畸形和规约检测，具体字段如下所示：

start\_byte

end\_byte

not\_MSH

unknow\_seg\_separator

exist\_invalid\_char

segment\_name\_len

msh\_field2\_len

msh\_field9\_len

not\_trigger\_event

not\_message\_type

mult\_MSH

segment\_name

message\_type

trigger\_event

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

start\_byte字段：start\_byte字段为0x0B时，数据帧无法解析，上报畸形告警日志

segment\_name字段：segment\_name字段超出定义范围时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> HL7协议start\_byte字段不为0x0B，HL7报文显示如下
>
> <img src="产品质量_li_img/media/image368.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image369.png" alt="" data-size="original">

规约检查日志

> HL7协议segment\_name超出定义范围，HL7报文显示如下
>
> <img src="产品质量_li_img/media/image370.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image371.png" alt="" data-size="original">

**1.5.2.26. HNC**

支持2个字段的畸形检测，具体字段如下所示：

HncHead\_length\_error

HncSpackHead\_length\_error

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

HncHead字段：HncHead字段的长度小于10时，数据帧无法解析，上报畸形告警日志

测试用例举例说明

畸形检查日志

> HNC协议HncHead的长度小于10，HNC报文显示如下
>
> <img src="产品质量_li_img/media/image372.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image373.png" alt="" data-size="original">

**1.5.2.27. Honeywell**

支持4个字段的畸形和规约检测，具体字段如下所示：

body\_len

item\_len

item\_seq\_no

item\_num

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

body\_len字段：body\_len字段值和实际body的长度不一致时，数据帧无法解析，上报畸形告警日志

item\_seq\_no字段：item\_seq\_no字段不连续递增时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Honeywell协议body\_len非法，Honeywell报文显示如下
>
> <img src="产品质量_li_img/media/image374.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image375.png" alt="" data-size="original">

规约检查日志

> Honeywell协议item\_seq\_no不连续递增，Honeywell报文显示如下
>
> <img src="产品质量_li_img/media/image376.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image377.png" alt="" data-size="original">

**1.5.2.28. HT2000R**

支持1个字段的规约检测，具体字段如下所示：

func\_code

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

func\_code字段：func\_code字段值未在取值范围0x05，0x06时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> HT2000R协议func\_code字段值未在取值范围0x05，0x06，HT2000R报文显示如下
>
> <img src="产品质量_li_img/media/image378.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image379.png" alt="" data-size="original">

**1.5.2.29. JX300**

支持2个字段的规约检测，具体字段如下所示：

FLAG

function\_code

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

FLAG字段：FLAG字段未在范围值(0/1)时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> JX300协议FLAG以及function\_code非法，JX300报文显示如下
>
> <img src="产品质量_li_img/media/image380.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image381.png" alt="" data-size="original">

**1.5.2.30. Melsec**

支持2个字段的畸形和规约检测，具体字段如下所示：

frame\_header

command

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

frame\_header字段：frame\_header字段不为0x5400、0xD400时，数据帧无法解析，上报畸形告警日志

command字段：command字段取值不在协议规范范围内时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

畸形检查日志

> Melsec协议frame\_header不在预定范围内，Melsec报文显示如下
>
> <img src="产品质量_li_img/media/image382.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image383.png" alt="" data-size="original">

规约检查日志

> Melsec协议command不在预定范围内，Melsec报文显示如下
>
> <img src="产品质量_li_img/media/image384.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image385.png" alt="" data-size="original">

**1.5.2.31. NA\_RTU**

支持2个字段的规约检测，具体字段如下所示：

preamble

func\_code

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Preamble字段：preamble字段值不为0x55时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> NA\_RTU协议preamble不为0x55，NA\_RTU报文显示如下
>
> <img src="产品质量_li_img/media/image386.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image387.png" alt="" data-size="original">

**1.5.2.32. Ovation\_TCP**

支持1个字段的规约检测，具体字段如下所示：

func\_code

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

func\_code字段：func\_code字段不为0x0008或0x000c或0x0010时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> Ovation\_TCP协议func\_code非法，Ovation\_TCP报文显示如下
>
> <img src="产品质量_li_img/media/image388.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image389.png" alt="" data-size="original">

**1.5.2.33. Profinetdcp**

支持2个字段的规约检测，具体字段如下所示：

ServiceID

SerivceType

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

ServiceID字段：ServiceID字段未在范围值(0x03, 0x04, 0x05, 0x06)时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> Profinetdcp协议ServiceID不在范围内，Profinetdcp报文显示如下
>
> <img src="产品质量_li_img/media/image390.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image391.png" alt="" data-size="original">

**1.5.2.34. Profinetmrp**

支持1个字段的规约检测，具体字段如下所示：

MRP\_TLVHeader.Type

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

MRP\_TLVHeader.Type字段：MRP\_TLVHeader.Type字段未在范围值(0x00,0x01,0x02,0x03,0x04,0x05,0x7f)时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> Profinetmrp协议MRP\_TLVHeader.Type未在范围内，Profinetmrp报文显示如下
>
> <img src="产品质量_li_img/media/image392.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image393.png" alt="" data-size="original">

**1.5.2.35. Profinetmrrt**

支持1个字段的规约检测，具体字段如下所示：

Type

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

Type字段：Type字段未在范围值(0x00,0x01,0x02)时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> Profinetmrrt协议Type未在范围内，Profinetmrrt报文显示如下
>
> <img src="产品质量_li_img/media/image394.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image395.png" alt="" data-size="original">

**1.5.2.36. Profinet\_PTCP**

支持1个字段的畸形检测，具体字段如下所示：

FrameID

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

FrameID字段：

1：FrameID在范围（frame\_id >= 0x0100 && frame\_id < 0xFF00或者frame\_id > 0xFF5F）内时,被识别为其他profinet协议进行解析

2：FrameID未在范围(（frame\_id >= 0x0100 && frame\_id < 0xFF00或者frame\_id > 0xFF5F)内，且未在范围(0x0020、0x0021、0x0080、0x0081、0xff00、0xff01、0xff20、0xff21、0xff40、0xff41、0xff42、0xff43)时，数据帧不可以正常解析，上报畸形告警日志

测试用例举例说明

畸形检查日志

> Profinet\_PTCP协议FrameID不符合条件，Profinet\_PTCP报文显示如下
>
> <img src="产品质量_li_img/media/image396.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image397.png" alt="" data-size="original">

**1.5.2.37. RSSP-1**

支持2个字段的规约检测，具体字段如下所示：

interaction\_type

protocol\_type

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

interaction\_type字段：interaction\_type未在范围值(0x01，0x02)时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> RSSP-1协议interaction\_type未在范围值，RSSP-1报文显示如下
>
> <img src="产品质量_li_img/media/image398.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image399.png" alt="" data-size="original">

**1.5.2.38. S7Plus**

支持3个字段的规约检测，具体字段如下所示：

ProtocolId

ProtocolVersion

Opcode

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

ProtocolId字段：ProtocolId不为值0x72时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> S7Plus 协议ProtocolId不为值0x72，S7Plus报文显示如下
>
> <img src="产品质量_li_img/media/image400.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image401.png" alt="" data-size="original">

**1.5.2.39. XHICAN**

支持2个字段的规约检测，具体字段如下所示：

preamble

command

畸形和规约检测的条件和标准

数据帧按照协议规范进行解析，如果数据格式错误导致解析失败，则上报对应的畸形告警日志，一个数据帧最多上报一个畸形告警日志。

数据帧按照协议规范进行解析，如果语义错误，则上报对应的规约告警日志，数据帧可以正常解析，一个数据帧可以上报多个规约告警日志。

畸形或规约数据帧不漏报畸形或规约告警日志，非畸形或规约数据帧不误报畸形或规约告警日志

例如：

preamble字段：preamble字段值取值非0x413541354135时，数据帧可以正常解析，上报规约告警日志

测试用例举例说明

规约检查日志

> XHICAN协议preamble不为0x413541354135，XHICAN报文显示如下
>
> <img src="产品质量_li_img/media/image402.png" alt="" data-size="original">
>
> ISTP Web显示结果如下图所示
>
> <img src="产品质量_li_img/media/image403.png" alt="" data-size="original">

### 1.6. 工业IPS

#### 1.6.1. 功能说明

工业IPS规则可以告警漏洞攻击，针对系统漏洞攻击的公开漏洞、私有漏洞、关键事件、协议异常等进行防护。

#### 1.6.2. 发布的标准

工业IPS功能支持8种工业协议、52款设备、32款软件的254个漏洞的入侵检测。

IPS引擎支持19种工业协议的入侵检测。

**1.6.2.1. S7**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

S7协议拒绝服务漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\test02.png](产品质量\_li\_img/media/image404.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\test01.png](产品质量\_li\_img/media/image405.png)

**1.6.2.2. MODBUS**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

MODBUS协议Restart Communications Option漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-03.jpg](产品质量\_li\_img/media/image406.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-01.jpg](产品质量\_li\_img/media/image407.png)

**1.6.2.3. DNP3**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

DNP3协议Cold Restart From Authorized Client漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-08.jpg](产品质量\_li\_img/media/image408.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-07.jpg](产品质量\_li\_img/media/image409.png)

**1.6.2.4. ENIP\_CIP**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

ENIP\_CIP协议Reset IP of ControlLogix\_1756-EN2TD漏洞攻击报文情况，如下图所示

![](产品质量\_li\_img/media/image410.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-09.jpg](产品质量\_li\_img/media/image411.png)

**1.6.2.5. OMRON**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

OMRON协议可编程逻辑控制器存在内存破坏型漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-14.png](产品质量\_li\_img/media/image412.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-13.png](产品质量\_li\_img/media/image413.png)

**1.6.2.6. MELSEC**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

MELSEC协议拒绝服务漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-16.png](产品质量\_li\_img/media/image414.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-15.png](产品质量\_li\_img/media/image415.png)

**1.6.2.7. IEC104**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

IEC104协议重置进程命令敏感操作漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\ISTP-340-指标10\截图\test-54.png](产品质量\_li\_img/media/image416.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\ISTP-340-指标10\截图\test-53.PNG](产品质量\_li\_img/media/image417.png)

**1.6.2.8. OPC\_DA**

IPS规则测试发布标准

> 可检测到IPS规则对应的漏洞攻击，产生威胁告警
>
> 威胁告警不产生漏报、误报的情况，告警显示内容与规则相匹配
>
> IPS规则可实现跨帧检测漏洞攻击

测试用例举例说明

OPC\_DA协议IOPCItemIO WriteVQT命令敏感操作漏洞攻击报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\ISTP-340-指标10\截图\test-56.png](产品质量\_li\_img/media/image418.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\ISTP-340-指标10\截图\test-55.png](产品质量\_li\_img/media/image419.png)

### 1.7. 异常行为检测

#### 1.7.1. 功能说明

多种协议字段的flood和scan攻击等异常行为的检测，目前支持15种协议的异常行为检测。

#### 1.7.2. 发布的标准

**1.7.2.1. DNP3**

支持的异常检测字段如下

| 字段ID | 字段名称        |
| ---- | ----------- |
| 1    | Function    |
| 2    | Source      |
| 3    | Destination |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

DNP3协议 “Function”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-18.png](产品质量\_li\_img/media/image420.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-19.png](产品质量\_li\_img/media/image421.png)

**1.7.2.2. ENIP\_CIP**

支持的异常检测字段如下

| 字段ID | 字段名称    |
| ---- | ------- |
| 1    | service |
| 2    | commond |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

ENIP\_CIP协议 “service”字段和“commond”字段异常行为检测报文情况，如下图所示

![](产品质量\_li\_img/media/image422.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-20.png](产品质量\_li\_img/media/image423.png)

**1.7.2.3. IEC104**

支持的异常检测字段如下

| 字段ID | 字段名称     |
| ---- | -------- |
| 1    | type\_id |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

IEC104协议“type\_id”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-24.png](产品质量\_li\_img/media/image424.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-23.png](产品质量\_li\_img/media/image425.png)

**1.7.2.4. Modbus\_TCP**

支持的异常检测字段如下

| 字段ID | 字段名称     |
| ---- | -------- |
| 1    | Function |
| 2    | address  |
| 3    | value    |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Modbus\_TCP协议“Function”字段、“address”字段和“value”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-26.png](产品质量\_li\_img/media/image426.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-25.png](产品质量\_li\_img/media/image427.png)

**1.7.2.5. Modbus\_UDP**

支持的异常检测字段如下

| 字段ID | 字段名称     |
| ---- | -------- |
| 1    | Function |
| 2    | address  |
| 3    | value    |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Modbus\_UDP协议“Function”字段、“address”字段和“value”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-28.png](产品质量\_li\_img/media/image428.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-27.png](产品质量\_li\_img/media/image429.png)

**1.7.2.6. Modbus\_UMAS**

支持的异常检测字段如下

| 字段ID | 字段名称     |
| ---- | -------- |
| 1    | Function |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Modbus\_UMAS协议“Function”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-29.png](产品质量\_li\_img/media/image430.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-30.png](产品质量\_li\_img/media/image431.png)

**1.7.2.7. OPC\_DA**

支持的异常检测字段如下

| 字段ID | 字段名称          |
| ---- | ------------- |
| 1    | Interface     |
| 2    | Function Code |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

OPC\_DA协议“Interface”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-32.png](产品质量\_li\_img/media/image432.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-31.png](产品质量\_li\_img/media/image433.png)

**1.7.2.8. S7**

支持的异常检测字段如下

| 字段ID | 字段名称          |
| ---- | ------------- |
| 1    | Function Code |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

S7协议“Function Code”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-33.png](产品质量\_li\_img/media/image434.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-34.png](产品质量\_li\_img/media/image435.png)

**1.7.2.9. HartIP**

支持的异常检测字段如下

| 字段ID | 字段名称       |
| ---- | ---------- |
| 1    | Command    |
| 2    | Frame Type |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

HartIP协议“Command”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-22.png](产品质量\_li\_img/media/image436.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-21.png](产品质量\_li\_img/media/image437.png)

**1.7.2.10. Profinet-DCP**

支持的异常检测字段如下

| 字段ID | 字段名称        |
| ---- | ----------- |
| 1    | ServiceType |
| 2    | ServiceID   |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-DCP协议“ServiceType”字段和“ServiceID”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-37.png](产品质量\_li\_img/media/image438.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-36.PNG](产品质量\_li\_img/media/image439.png)

**1.7.2.11. Profinet-MRP**

支持的异常检测字段如下

| 字段ID | 字段名称 |
| ---- | ---- |
| 1    | Type |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-MRP协议“Type”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-39.png](产品质量\_li\_img/media/image440.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-38.PNG](产品质量\_li\_img/media/image441.png)

**1.7.2.12. Profinet-MRRT**

支持的异常检测字段如下

| 字段ID | 字段名称 |
| ---- | ---- |
| 1    | Type |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-MRRT协议“Type”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-40.png](产品质量\_li\_img/media/image442.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-41.PNG](产品质量\_li\_img/media/image443.png)

**1.7.2.13. Profinet-PTCP**

支持的异常检测字段如下

| 字段ID | 字段名称       |
| ---- | ---------- |
| 1    | SequenceID |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-PTCP协议“SequenceID”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-42.png](产品质量\_li\_img/media/image444.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-43.png](产品质量\_li\_img/media/image445.png)

**1.7.2.14. Profinet-RTC1**

支持的异常检测字段如下

| 字段ID | 字段名称         |
| ---- | ------------ |
| 1    | data\_status |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-RTC1协议“data\_status”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-44.png](产品质量\_li\_img/media/image446.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-45.png](产品质量\_li\_img/media/image447.png)

**1.7.2.15. Profinet-RTC3**

支持的异常检测字段如下

| 字段ID | 字段名称         |
| ---- | ------------ |
| 1    | data\_status |

异常行为检测发布标准

> 畸形请求帧不上报异常行为检测
>
> flood攻击1s内攻击报文相同字段大于阈值设定可产生异常检测告警，不产生漏报和误报的情况
>
> scan攻击1s内攻击报文大于5个不同字段可产生异常检测告警，不产生漏报和误报的情况

测试用例举例说明

Profinet-RTC3协议“data\_status”字段异常行为检测报文情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-49.png](产品质量\_li\_img/media/image448.png)

ISTP检测情况，如下图所示

![C:\Users\zhengqiang01\Desktop\ISTP-第8期结项相关工作\test-48.png](产品质量\_li\_img/media/image449.png)

### 1.8. 资产被动识别

#### 1.8.1. 功能说明

资产被动识别通过对数据包中的资产指纹特征进行检测分析，检测流量中是否包含与预置资产特征相匹配的资产信息，从而实现对工业资产的识别。

#### 1.8.2. 发布的标准

ISTP支持47厂商129款设备的识别，如下表所示。支持1种识别方式。

| 序号  | 厂商                  | 资产                                                        |
| --- | ------------------- | --------------------------------------------------------- |
| 1   | 3S                  | 3s.CODESYS                                                |
| 2   | ABB                 | ABB.AC800F.PM802F                                         |
| 3   |                     | ABB.AC800M.PM856                                          |
| 4   |                     | ABB AC500.PM573-ETH                                       |
| 5   | ADVANTECH           | ADVANTECH.ADAM-4571L-DE                                   |
| 6   |                     | ADVANTECH.ADAM-5510EKW/TP                                 |
| 7   | Beckhoff            | Beckhoff.CX.CX1500-M310                                   |
| 8   |                     | Beckhoff.CX8000.CX8091                                    |
| 9   | BR                  | BR.X20.CP1484                                             |
| 10  |                     | B\&R.X20.X20CP1301                                        |
| 11  | COTRUST             | COTRUST.CTH300-H.CTH3 H31-000S1                           |
| 12  | Delta               | Delta.DVP-ES2.DVP20ES200TE                                |
| 13  | DCCE                | DCCE.MAC.MAC1000ProgramableController                     |
| 14  |                     | DCCE.MAC.MAC1100                                          |
| 15  | Etrol               | Etrol.RTU\_PLC.Super32                                    |
| 16  |                     | Etrol.RTU.SuperE32L601                                    |
| 17  |                     | Etrol.super32.L206                                        |
| 18  |                     | Etrol.RTU.SL304                                           |
| 19  | Emerson             | Bristol Babcock.ControlWave® Micro                        |
| 20  |                     | Emerson.ROC800.CPU Series 2                               |
| 21  |                     | Emerson.DELTAV.MQ controller. CTLR-32DD94 KJ2005X1-MQ2    |
| 22  | Fanuc               | FANUC.Series 0i                                           |
| 23  | Sunway ForceControl | Sunway ForceControl                                       |
| 24  | GE                  | GE.VerMax\_IC200CPUE05.Private                            |
| 25  |                     | PAC\_RX3iIC695CPE302                                      |
| 26  | HIKVSION            | DS-IPC-B12V2-I                                            |
| 27  | HIKVSION(萤石）        | CS-C3W-1C2WFR                                             |
| 28  | HITACHI             | HITACHI.MICRO-EHV.MVH-A40DR                               |
| 29  | HollySys            | HollySys.DCS.MACS                                         |
| 30  |                     | HollySys.NuclearPower.HEROS\_RTS                          |
| 31  |                     | HollySys.NuclearPower.NB220                               |
| 32  |                     | HollySys.NuclearPower.NM-DP                               |
| 33  |                     | HollySys.NuclearPower.NM220                               |
| 34  |                     | HollySys.PLC.LK220                                        |
| 35  |                     | HOLLiAS MACS-K.K-CU01                                     |
| 36  | HoneyWell           | Honey.Controller.C300                                     |
| 37  |                     | Honey.Firewall.FTE\_Control\_Firewall                     |
| 38  | HUATONG             | HUATONG.2000R\_CS                                         |
| 39  | IDEC(和泉)            | IDEC(和泉).MicroSmart\_FC6A.FC6A-D16R4CEE                   |
| 40  | Inovance            | Inovance.AM600.AM600-CPU1608TP                            |
| 41  | KEYENCE(基恩士)        | KEYENCE.KV-7000.KV-7500                                   |
| 42  | KLAND               | Newpre3000Newpre3000-P121-M3-D1-G0                        |
| 43  | Koyo(光洋)            | kostacSJ-12DD2EP-D                                        |
| 44  | Kinco               | Kinco.K2.CPU204ET.K204ET-16DT                             |
| 45  | LT                  | LT.GJ303.GHMSL                                            |
| 46  | MITSUBISHI          | MITSUBISHI.LCPU.L06CPU                                    |
| 47  |                     | MITSUBISHI.MELSEC-L.L02CPU                                |
| 48  |                     | MITSUBISHI.QCPU.Q02HCPU                                   |
| 49  |                     | MITSUBISHI.QCPU.Q03UDECPU                                 |
| 50  |                     | MITSUBISHI.MELSEC-FX5U-32MR/ES                            |
| 51  | Moxa                | Moxa.EDS-405A                                             |
| 52  |                     | NPort52005230                                             |
| 53  |                     | MOXA.RemoteIO.E1242                                       |
| 54  | NA                  | NA.PLC.CPU401-0401                                        |
| 55  |                     | NA.RTU.CPU401.1101                                        |
| 56  |                     | NA200H.CPU201-1101                                        |
| 57  |                     | NA400.CPU401-0201                                         |
| 58  | OMRON               | OMRON.CJ2M.CPU31                                          |
| 59  |                     | OMRON.CP.CP1H-XA40DT-D                                    |
| 60  |                     | Omron.CP.CP1H.XA40DR\_A                                   |
| 61  |                     | OMRON.CJ2M.CJ2M-CPU35                                     |
| 62  |                     | OMRON.CP.CP1L-EL20DR-D                                    |
| 63  |                     | Omron.CP1L-EL20DT-D                                       |
| 64  |                     | Omron.CP1L-EM40DR-D                                       |
| 65  | OPTO22              | OPTO22.SNAP PAC R.SNAP-PAC-R2                             |
| 66  | Phoenix             | Phoenix.100.ILC330ETH                                     |
| 67  | 　                   | Phoenix.Inline.ILC131 ETH                                 |
| 68  | Progea              | ProgeaMovicon Power HMI                                   |
| 69  | RedLine             | redlion-crimson3\_Crimson3                                |
| 70  |                     | RedLion.Graphite.GRAC0001                                 |
| 71  | RockWell\_AB        | RockWell\_AB.CompactLogix\_1769-L33ER                     |
| 72  |                     | RockWell\_AB.CompactLogix\_1769-L35E                      |
| 73  |                     | RockWell\_AB.ControlLogix\_1756\_EN2T\_C                  |
| 74  |                     | RockWell\_AB.ControlLogix\_1756-EN2T\_D                   |
| 75  |                     | RockWell\_AB.ControlLogix\_1756-EN2T\_D\_CASIA            |
| 76  |                     | RockWell\_AB.Controllogix.1756-L71/B Logix5571            |
| 77  |                     | RockWell\_AB.CompactLogix 5380.5069-L306ER                |
| 78  |                     | RockWell\_AB.Micro800.Micro850.2080-LC50-24QWB            |
| 79  |                     | RockWell\_AB.Micrologix14001766-L32BWA                    |
| 80  |                     | RockWell\_AB.SLC 5\_05 CPU.1747-L551C                     |
| 81  |                     | RockWell\_AB.SoftLogix5800.1789-L60/A                     |
| 82  |                     | RockWell\_AB.1756-ENBT/A                                  |
| 83  | Schneider           | Schneider.M218\_LDAE40DRPHN                               |
| 84  |                     | Schneider.M340\_BMXP342020（M340\_CPU340-20）               |
| 85  |                     | Schneider.M340.NOE0100                                    |
| 86  |                     | Schneider.M340\_BMXP3420102                               |
| 87  |                     | Schneider.M580.BMEP582040                                 |
| 88  |                     | Schneider.Quantum\_CPU\_31110                             |
| 89  |                     | Schneider.Quantum\_CPU\_65150                             |
| 90  |                     | Schneider.Premium.TSXP571634M                             |
| 91  |                     | Schneider.Vijeo Citect                                    |
| 92  | Siemens             | Siemens.CP\_343-1\_advanced                               |
| 93  |                     | Siemens.CP\_343-1                                         |
| 94  |                     | Siemens.CP\_443-1\_advanced                               |
| 95  |                     | Siemens.CP\_443-1                                         |
| 96  |                     | Siemens.CP\_1543-1                                        |
| 97  |                     | Siemens.S7-200\_SMART.CPU\_ST20                           |
| 98  |                     | Siemens.S7\_200\_Smart\_CPU\_st30                         |
| 99  |                     | Siemens.S7\_200\_Smart\_CPU\_st40                         |
| 100 |                     | Siemens.s7\_200 \_smart.CPU SR30                          |
| 101 |                     | Siemens.S7\_300\_CPU\_314c-2\_PNDP                        |
| 102 |                     | Siemens.S7\_300\_CPU\_314c-2                              |
| 103 |                     | Siemens.S7\_300\_CPU\_315-2\_PNDP                         |
| 104 |                     | Siemens.S7\_300\_CPU\_315F-2                              |
| 105 |                     | Siemens.S7\_300\_CPU\_317-2\_PNDP                         |
| 106 |                     | Siemens.S7\_400\_CPU\_412-5h\_PNDP                        |
| 107 |                     | Siemens.S7\_400\_CPU\_412-5H                              |
| 108 |                     | Siemens.S7\_400\_CPU\_414-5h                              |
| 109 |                     | Siemens.S7-400\_CPU417-5H PN/DP                           |
| 110 |                     | Siemens.S7\_1200\_CPU\_1212c\_DCDCRly                     |
| 111 |                     | Siemens.SIMATIC S7-1500.CPU 1515-2 PN.6ES7 515-2AM02-0AB0 |
| 112 |                     | Siemens.S7\_1200\_CPU\_1214C\_ACDCRLY                     |
| 113 |                     | Siemens.S7\_1200\_CPU\_1214c\_DCDCDC                      |
| 114 |                     | Siemens.S7\_1200\_CPU\_1215c\_DCDCDC                      |
| 115 |                     | Siemens.S7-1500\_CPU\_1516-3\_PNDP（CP 1516\_3）            |
| 116 |                     | Siemens.SINUMERIK\_808D                                   |
| 117 |                     | Siemens.HMI.smartline.1000v3 ie                           |
| 118 | Supcon              | Supcon.GCS.GCS-3                                          |
| 119 |                     | Supcon.JX-300                                             |
| 120 |                     | Supcon.TCS-900(SCnet100)                                  |
| 121 | WAGO                | WAGO.750.750-832                                          |
| 122 | XINHUA              | XINHUA.XDC800.XCU-net                                     |
| 123 | Yokogawa            | Yokogawa.FACTORY ACE.F3LE12-1T.(F3SP22-OS)                |
| 124 | 大华                  | 大华.TP7                                                    |
| 125 | 国电智深                | 国电智深.DCS.EDPF-DPU3（GPS）                                   |
| 126 | 腾控科技                | 腾控科技.T900.T920                                            |
| 127 | 燕山电子                | Yanshan.401.008                                           |
| 128 | 亚控科技                | KingView                                                  |
| 129 | KEP                 | KEP.ware.KEP.ServerEx.V.4                                 |

ISTP识别的资产信息维度包括资产IP地址、MAC 地址、厂商、系列、型号。

发布标准

> 开发实现范围内的资产，可正常识别，不存在误识别、不识别情况
>
> 识别的资产信息及维度（IP地址、MAC 地址、厂商、系列、型号）与实际流量指纹特征相匹配

测试用例举例说明

> 以资产ABB.AC800M.PM856识别为例，报文内容如下图所示。
>
> <img src="产品质量_li_img/media/image450.png" alt="" data-size="original">
>
> ISTP识别结果，如下图所示。
>
> <img src="产品质量_li_img/media/image451.png" alt="" data-size="original">

### 1.9. 资产主动识别

#### 1.9.1. 功能说明

通过主动识别收发报文引擎功能，检测流量中是否包含与资产相匹配的资产信息，从而实现对目标设备的资产主动识别探测功能。

#### 1.9.2. 发布的标准

资产主动识别功能支持基于61种协议来识别60个厂商的121款设备，支持1种识别方式，支持17种服务类型。

富化信息识别功能支持30种协议来识别26个厂商的50款设备。

资产信息包含类型、厂商、系列、设备型号、设备类型、硬件版本、固件版本等。

资产主动识别测试发布标准

> 可识别到资产信息，资产识别结果与实际流量特征相匹配
>
> 资产信息稳定识别，不存在二进制插件执行报错问题

测试用例举例说明

> Schneider.Modicon M580设备报文情况，如下图所示
>
> <img src="产品质量_li_img/media/image452.png" alt="" data-size="original">
>
> Schneider.Modicon M580设备资产主动识别情况，如下图所示

![](产品质量\_li\_img/media/image453.png)

### 1.10. 漏洞映射

#### 1.10.1. 功能说明

通过资产信息匹配cpe工业漏洞信息库中的漏洞信息，可通过设备型号和固件版本信息匹配漏洞。

#### 1.10.2. 发布的标准

漏洞映射功能支持4691个漏洞的映射

漏洞映射功能支持2种漏洞映射方式

> 通过设备型号和固件版本信息映射设备当前版本的漏洞信息
>
> 通过设备型号映射设备所有固件版本的漏洞信息

漏洞映射测试发布标准

> 可识别到设备相关漏洞列表信息，漏洞映射结果不存在错误信息
>
> 使用不同版本信息漏洞映射的结果应与cpe工业漏洞信息库中的漏洞信息相匹配

测试用例举例说明

Siemens.S7-300.CPU315-2 PN/DP设备不同版本漏洞映射情况，如下图所示

![](产品质量\_li\_img/media/image454.png)

![](产品质量\_li\_img/media/image455.png)

## 2. 健壮性

目前针对ISTP各模块的健壮性质量特性进行了健壮性测试（特别是协议相关模块）。为确保ISTP各模块的健壮性符合标准，在测试过程中利用Fuzzing等测试技术来构造有针对性的异常输入数据。

目前ISTP通过了绿盟漏扫、中京漏挖、博智漏挖等多款产品在OPC UA、FINS、DNP3、CIP等32种协议模块的Fuzzing测试，同时通过了OPC DA、Focas、CIP PCCC等15种协议基于白名单和畸形字段的72种变形的针对性健壮性测试，测试未发现dp挂死等阻断性问题，符合健壮性发布标准，涉及的协议如下表所示。

| **协议**              | **绿盟漏扫** | **中京漏挖** | **博智漏挖** | **Peach** | **BooFuzz** | **beStorm** | **kittyfuzz** | **科来** |
| ------------------- | -------- | -------- | -------- | --------- | ----------- | ----------- | ------------- | ------ |
| **OPC DA**          |          |          |          | √         |             |             |               | √      |
| **Focas**           |          |          |          | √         |             |             |               |        |
| **CIP PCCC**        |          |          |          | √         |             |             |               |        |
| **CIP Logix5000**   |          |          |          | √         |             |             |               |        |
| **BACnet**          |          |          | √        |           | √           |             |               |        |
| **CIP**             |          |          | √        |           |             |             |               |        |
| **DNP3-TCP**        | √        | √        | √        |           |             |             |               |        |
| **DNP3-UDP**        |          |          | √        |           |             |             |               |        |
| **Ethernet/IP-TCP** |          | √        | √        |           |             |             |               |        |
| **Ethernet/IP-UDP** |          |          | √        |           |             |             |               |        |
| **FINS-TCP/UDP**    |          |          | √        |           |             |             |               |        |
| **GOOSE**           |          |          | √        |           |             |             |               |        |
| **IEC104**          | √        | √        | √        |           |             |             |               |        |
| **MMS**             | √        | **√**    | √        |           |             |             |               |        |
| **Modbus TCP**      | √        | √        | √        | √         | √           | √           | √             |        |
| **Modbus UDP**      |          |          |          | √         |             |             |               |        |
| **Modbus UMAS**     |          |          |          | √         |             |             |               |        |
| **OPC UA**          |          | √        | √        |           |             |             |               |        |
| **Profinet DCP**    | √        |          | √        |           |             |             |               |        |
| **Profinet MRP**    |          |          | √        |           |             |             |               |        |
| **Profinet PTCP**   |          |          |          | √         |             |             |               |        |
| **S7-Plus**         |          |          |          | √         |             |             |               |        |
| **SV**              |          |          | √        |           |             |             |               |        |
| **HartIP\_TCP/UDP** |          |          | √        | √         |             |             |               |        |
| **NRIEC103**        |          |          |          | √         |             |             |               |        |
| **MELSEC TCP**      |          | √        |          | √         |             |             |               |        |
| **RSSP-1**          |          |          |          | √         |             |             |               |        |
| **S7**              | √        | √        | √        | √         |             |             |               |        |
| **HTTP**            |          | √        |          | √         |             |             |               |        |
| **S7**              | √        | √        | √        | √         |             |             |               |        |
| **Modbus RTU**      |          |          |          |           |             |             |               | √      |
| **Modbus ASCII**    |          |          |          |           |             |             |               | √      |

## 3. 稳定性

目前针对ISTP的如下功能模块的稳定性质量特性进行了长期稳定测试，在为期3天/周的长期测试下，内存占用率约30%、cpu占用率约为40%，丢包率为2%以下；各轮次测试结果均保持一致，未出现功能使用阻塞性问题。

协议识别：包含140种协议

协议解析：包含49种协议

协议白名单：包含49种协议

畸形和规约检测：包含39种协议

关键事件：包含31种协议共计353个关键事件

工业IPS：包含254条IPS规则

资产被动识别：包含47个厂商129款资产

## 4. 产品兼容性

目前ISTP各模块已合入工业防火墙、ISD、工业网闸、漏扫、IETC、移动堡垒机等数款产品的多个版本，且已通过工业防火墙、IETC、ISD、漏扫等产品的联调测试，目前相关产品可正常工作。
