# ISTP功能综述

### 集成协议和对应功能列表

| 序号 | 协议名称                | 深度解析 | 白名单 | 畸形包检测 | 关键事件 | 点表-值域 | 异常 | 文件还原 | 时效白名单 | 备注 |
| -- | ------------------- | ---- | --- | ----- | ---- | ----- | -- | ---- | ----- | -- |
| 1  | MMS                 | Y    | Y   | Y     | Y    |       |    | Y    |       |    |
| 2  | BACNET              | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 3  | CoAp                | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 4  | DNP3 TCP            | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 5  | DNP3 UDP            | Y    | Y   |       |      |       |    |      |       |    |
| 6  | ENIP                | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 7  | CIP\_COMMON         | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 8  | CIP\_Logix5000      | Y    | Y   |       |      |       |    |      |       |    |
| 9  | CIP\_PCCC           | Y    | Y   |       | Y    |       |    |      |       |    |
| 10 | Etrol\_SL304\_TCP   | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 11 | Focas               | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 12 | GDW 3761            | Y    | Y   | Y     |      |       |    |      |       |    |
| 13 | GOOSE               | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 14 | HartIP\_TCP         | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 15 | HartIP\_UDP         | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 16 | HuaTong\_2000R\_TCP | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 17 | IEC104              | Y    | Y   | Y     | Y    | Y     | Y  | Y    |       |    |
| 18 | JX300               | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 19 | MELSEC\_TCP         | Y    | Y   | Y     | Y    | Y     |    |      |       |    |
| 20 | Modbus\_TCP         | Y    | Y   | Y     | Y    | Y     | Y  |      | Y     |    |
| 21 | Modbus\_UDP         | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 22 | Modbus\_UMAS        | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 23 | Modbus\_RTU         | Y    | Y   |       |      |       |    |      |       |    |
| 24 | MQTT                | Y    | Y   |       |      |       |    |      |       |    |
| 25 | NA\_RTU\_TCP        | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 26 | OMRON\_TCP          | Y    | Y   | Y     | Y    | Y     |    |      |       |    |
| 27 | OMRON\_UDP          | Y    | Y   | Y     | Y    | Y     |    |      |       |    |
| 28 | OPC\_DA             | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 29 | OPC\_UA             | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 30 | ovation\_tcp        | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 31 | Profinet\_DCP       | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 32 | Profinet\_MRP       | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 33 | Profinet\_MRRT      | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 34 | Profinet\_PTCP      | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 35 | Profinet\_RTC1      | Y    | Y   | Y     |      |       | Y  |      |       |    |
| 36 | Profinet\_RTC3      | Y    | Y   | Y     | Y    |       | Y  |      |       |    |
| 37 | RSSP-1              | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 38 | S7                  | Y    | Y   | Y     | Y    | Y     | Y  |      |       |    |
| 39 | S7\_Plus            | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 40 | GE\_SRTP            | Y    | Y   | Y     |      |       |    |      |       |    |
| 41 | SV                  | Y    | Y   | Y     | Y    |       |    |      |       |    |
| 42 | Shanghaixinhua\_DCS | Y    | Y   | Y     |      |       |    |      |       |    |
| 43 | IEC103\_UDP（NR）     | Y    | Y   |       |      |       |    |      |       |    |

### 协议识别

工业协议识别支持100+种，工业协议解析支持34种。

工业协议解析具体能力，详见下方列表。

| **ID** | **协议名称**        |
| ------ | --------------- |
| 1      | mms             |
| 2      | bacnet          |
| 3      | coap            |
| 4      | dnp3            |
| 5      | enip            |
| 6      | etrolsl304tcp   |
| 7      | focas           |
| 8      | gdw3761         |
| 9      | goose           |
| 10     | hartip          |
| 11     | ht2000rtcp      |
| 12     | iec104          |
| 13     | jx300           |
| 14     | melsec          |
| 15     | modbus          |
| 16     | mqtt            |
| 17     | nartuoiltcp     |
| 18     | omron           |
| 19     | opcda           |
| 20     | opcua           |
| 21     | ovation         |
| 22     | profinetdcp     |
| 23     | profinetmrp     |
| 24     | profinetmrrt    |
| 25     | profinetptcp    |
| 26     | profinetrtc1    |
| 27     | profinetrtc3    |
| 28     | rssp\_1         |
| 29     | s7comm          |
| 30     | s7plus          |
| 31     | srtp            |
| 32     | sv              |
| 33     | xhican          |
| 34     | nr\_iec103\_udp |

### 协议解析白名单

工业协议解析白名单支持34种协议。

工业协议解析白名单具体支持能力，详见下方列表。

| **ID** | **协议名称**        |
| ------ | --------------- |
| 1      | mms             |
| 2      | bacnet          |
| 3      | coap            |
| 4      | dnp3            |
| 5      | enip            |
| 6      | etrolsl304tcp   |
| 7      | focas           |
| 8      | gdw3761         |
| 9      | goose           |
| 10     | hartip          |
| 11     | ht2000rtcp      |
| 12     | iec104          |
| 13     | jx300           |
| 14     | melsec          |
| 15     | modbus          |
| 16     | mqtt            |
| 17     | nartuoiltcp     |
| 18     | omron           |
| 19     | opcda           |
| 20     | opcua           |
| 21     | ovation         |
| 22     | profinetdcp     |
| 23     | profinetmrp     |
| 24     | profinetmrrt    |
| 25     | profinetptcp    |
| 26     | profinetrtc1    |
| 27     | profinetrtc3    |
| 28     | rssp\_1         |
| 29     | s7comm          |
| 30     | s7plus          |
| 31     | srtp            |
| 32     | sv              |
| 33     | xhican          |
| 34     | nr\_iec103\_udp |

### 关键事件-协议

关键事件-协议支持18种协议，涵盖16个厂商40款设备179种关键事件。

关键事件-协议具体支持能力，详见下方列表。

* 以协议统计如下：

| **ID** | **协议名称**   |
| ------ | ---------- |
| 1      | S7 COMM    |
| 2      | S7 Plus    |
| 3      | Modbus     |
| 4      | CIP        |
| 5      | MMS        |
| 6      | IEC104     |
| 7      | Omron      |
| 8      | Mitsubishi |
| 9      | DNP3       |
| 10     | OPC\_DA    |
| 11     | OPC\_UA    |
| 12     | RSSP-1     |
| 13     | Goose      |
| 14     | JX300      |
| 15     | PN DCP     |
| 16     | PN MRP     |
| 17     | PN MRRT    |
| 18     | PN PTCP    |

* 以厂商及设备统计如下：

| **ID** | **厂商**     | **设备数量** | 1 | 2 | 3 | 4 | **关键事件数量** |
| ------ | ---------- | -------- | - | - | - | - | ---------- |
| 1      | Siemens    | 10       |   |   |   |   | 66         |
| 2      | Schneider  | 6        |   |   |   |   | 36         |
| 3      | RockWell   | 4        |   |   |   |   | 12         |
| 4      | GE         | 1        |   |   |   |   | 1          |
| 5      | ABB        | 1        |   |   |   |   | 6          |
| 6      | OMRON      | 4        |   |   |   |   | 26         |
| 7      | MITSUBISHI | 3        |   |   |   |   | 0          |
| 8      | FANUC      | 1        |   |   |   |   | 3          |
| 9      | HollySys   | 3        |   |   |   |   | 0          |
| 10     | 上海新华       | 1        |   |   |   |   | 4          |
| 11     | 丹东华通       | 1        |   |   |   |   | 9          |
| 12     | 南大傲拓       | 1        |   |   |   |   | 10         |
| 13     | 安控         | 1        |   |   |   |   | 6          |
| 14     | 杭州海兴       | 1        |   |   |   |   | 0          |
| 15     | 海为         | 1        |   |   |   |   | 0          |
| 16     | Delta      | 1        |   |   |   |   | 0          |

### 资产被动识别

工业资产被动识别支持25 个厂商，88个系列，1599款设备。

工业资产被动识别具体支持能力，详见下方列表。（资产列表数量1451？数据有出入）

| ID | 厂商           | 资产数量 |
| -- | ------------ | ---- |
| 1  | Siemens      | 236  |
| 2  | Schneider    | 195  |
| 3  | Rockwell(AB) | 208  |
| 4  | GE           | 90   |
| 5  | ABB          | 51   |
| 6  | OMRON        | 53   |
| 7  | MITSUBISHI   | 43   |
| 8  | beckhoff     | 143  |
| 9  | B\&R         | 96   |
| 10 | MOXA         | 10   |
| 11 | RuggedCom    | 1    |
| 12 | Chitic(中自)   | 1    |
| 13 | Advantech    | 1    |
| 14 | Fanuc        | 80   |
| 15 | HoneyWell    | 2    |
| 16 | RedLine      | 1    |
| 17 | Phoenix      | 39   |
| 18 | Supcon       | 9    |
| 19 | HollySys     | 60   |
| 20 | 大工计控         | 25   |
| 21 | 蓝天数控         | 45   |
| 22 | 安控           | 19   |
| 23 | 南大奥拓         | 29   |
| 24 | OPTO22       | 12   |
| 25 | SCIYON(科远)   | 2    |

### 资产主动识别

工业资产主动识别类型包括硬件、软件、服务及IOT四种。

* 硬件资产识别支持43个厂商，63个系列，72款设备
* 软件资产识别支持14个厂商，14个系列，14款设备
* 服务识别支持14个厂商，46个系列，46款设备
* IOT资产识别支持6个厂商，7个系列，7款设备

工业资产主动识别具体支持能力，详见下方列表。

| **类型** | **厂商（支持系列数目）**                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 硬件     | <p>ABB(1);北京安控(1);HITASHI(1);YASKAWA(1); YOKOGAWA(1); ADVANTECH(3);</p><p>Etrol(1);Emerson(1); GE(1);HUATONG(1);Haiwell(2);INOVANCE(1);KEYENCE(1);</p><p>KLAND(2);MITSUBISH(3);Moxa(4);NATEKON(3);Omron(2);OPTO22(1);</p><p>Panasonic(1);Phoenix(1);RedLion(2);RockWell(6);WAGO(1);DELTA(1);XINJE(1);</p><p>FATEK(1);LSJS(1);HollySys(2);COTRUST(1);B&#x26;R(1);腾控科技(1);Kinco(1);</p><p>SUPCON(1); Schneider(3);Siemens(5);Elecom(0);Zlan(1);DEIF(1);ISE(0);MCGS(1); 燕山(1);</p> |
| 软件     | <p>Advantech(webaccess);Wellintech(kingview);ForceControl(ForceControl);</p><p>康吉森(Triview);Progea(Movicon);昆仑通态(MCGS);北京亚控科技(King SCADA);</p><p>Wonderware(InTouch);Schneider Vijeo(Citect);杰控(FameView);易控(INSPEC);</p><p>3s(CODESYS);GE Proficy(IFIX);Allen-Bradley (factorytalk view SE);</p>                                                                                                                                                                               |
| 服务     | <p>MODBUS TCP(TCP:502);BACNet(UDP:47808);IEC104(TCP:2404);</p><p>DNP3(TCP:20000);ECOM(UDP:28784);FINS(TCP:9600|UDP:9600);MELSEC Q(TCP|UDP:5000-5010);SNMP(UDP:161);ENIP(TCP:44818);S7(TCP:102);</p><p>MMS(TCP:102);GOOSE(eth);PROFINET(UDP:34964eth);CrimsonV3(TCP:789);</p><p>FOX(TCP:1911);PCWorX(TCP:1962);ProConOs(TCP:20547);OPC(TCP:135);</p><p>SV(eth);HARTIP(TCP:5094|UDP:5094);CODESYS(TCP:2455);SRTP(TCP:18245);</p><p>NPORT(UDP:4800);</p>                           |
| IOT    | 珠海思创(1);海康威视(2);大华(1);麦斯(1);研华(1);华为(1)                                                                                                                                                                                                                                                                                                                                                                                                                                         |

### 漏洞映射

ISTP已实现可识别资产的漏洞映射，包括公开漏洞及非公开漏洞，工业漏洞数量达5000+。

### 异常行为检测

异常行为检测支持6种协议的scan、flood攻击检测。

异常行为检测具体支持能力，详见下方列表。

| **ID** | **协议名称** |
| ------ | -------- |
| 1      | dnp3     |
| 2      | enip     |
| 3      | iec104   |
| 4      | modbus   |
| 5      | opcda    |
| 6      | s7comm   |

### 畸形包检测

畸形包检测支持13种工业协议。

畸形包检测具体支持能力，详见下方列表。

| **ID** | **协议名称**        |
| ------ | --------------- |
| 1      | mms             |
| 2      | bacnet          |
| 3      | dnp3            |
| 4      | enip            |
| 5      | goose           |
| 6      | iec104          |
| 7      | modbus          |
| 8      | omron           |
| 9      | opcda           |
| 10     | opcua           |
| 11     | s7comm          |
| 12     | sv              |
| 13     | nr\_iec103\_udp |

### 工业IPS

工业IPS规则实现194条，具体实现能力，详见下表

| **ID** | **类别** | **规则数量** |               |
| ------ | ------ | -------- | ------------- |
| 1      | 硬件     | 124条     | 19款PLC+8种工业协议 |
| 2      | 软件     | 57条      | 27款软件         |
| 3      | 其他     | 13条      | /             |

支持30+种IPS工业协议引擎，具体支持能力，详见下表

| **ID** | **协议**         |
| ------ | -------------- |
| 1      | S7COMM         |
| 2      | IEC104         |
| 3      | MQTT           |
| 4      | OMRON\_TCP     |
| 5      | OMRON\_UDP     |
| 6      | SUPCON         |
| 7      | COAP\_UDP      |
| 8      | DNP3           |
| 9      | OPC            |
| 10     | MODBUS\_TCP    |
| 11     | MODBUS\_UDP    |
| 12     | MODBUS\_UMAS   |
| 13     | MODBUS\_ASCII  |
| 14     | MODBUS\_RTU    |
| 15     | ENIP\_CIP      |
| 16     | MELSEC\_TCP    |
| 17     | MELSEC\_Q\_UDP |
| 18     | HartIP\_TCP    |
| 19     | HartIP\_UDP    |
| 20     | BACNET\_UDP    |
| 21     | FOCAS          |
| 22     | MMS            |
| 23     | RSSP\_1        |
| 24     | SRTP           |
| 25     | PROFINETDCP    |
| 26     | PROFINETMRP    |
| 27     | PROFINETPTCP   |
| 28     | PROFINETMRRT   |
| 29     | PROFINETRTC1   |
| 30     | PROFINETRTC3   |
| 31     | OPC\_UA        |
| 32     | DNP3\_UDP      |
