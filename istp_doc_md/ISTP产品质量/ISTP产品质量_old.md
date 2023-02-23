# ISTP产品质量

目前从功能性、健壮性、稳定性、产品兼容性等方面针对ISTP的质量特性来测试和把控

## 功能性

目前针对ISTP功能性质量特性进行了功能覆盖测试，测试场景覆盖度达到功能全覆盖。

ISTP各模块功能覆盖测试结果：通过，满足ISTP各模块的功能需求指标

### 测试场景覆盖

<table>
<colgroup>
<col style="width: 10%" />
<col style="width: 24%" />
<col style="width: 64%" />
</colgroup>
<thead>
<tr class="header">
<th>序号</th>
<th>功能模块名</th>
<th>测试说明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><ol type="1">
<li></li>
</ol></td>
<td>协议识别</td>
<td>120种协议通过协议识别功能的全覆盖测试</td>
</tr>
<tr class="even">
<td><ol start="2" type="1">
<li></li>
</ol></td>
<td>协议解析/白名单</td>
<td>40余种工业协议通过深度解析功能的全覆盖测试</td>
</tr>
<tr class="odd">
<td><ol start="3" type="1">
<li></li>
</ol></td>
<td>点表建模</td>
<td>4种工业协议通过点表建模功能的全覆盖测试</td>
</tr>
<tr class="even">
<td><ol start="4" type="1">
<li></li>
</ol></td>
<td>关键事件</td>
<td>20余种工业协议通过关键事件功能的全覆盖测试；同时通过30余款工控设备的关键事件功能全覆盖测试</td>
</tr>
<tr class="odd">
<td><ol start="5" type="1">
<li></li>
</ol></td>
<td>畸形包检测</td>
<td>20余种工业协议通过畸形包检测功能的全覆盖测试</td>
</tr>
<tr class="even">
<td><ol start="6" type="1">
<li></li>
</ol></td>
<td>入侵检测-IPS</td>
<td>30余种工业协议通过IPS工业协议引擎的全覆盖测试；同时通过180余条IPS规则的准确性测试</td>
</tr>
<tr class="odd">
<td><ol start="7" type="1">
<li></li>
</ol></td>
<td>异常行为检测</td>
<td>10余种工业协议通过异常行为检测功能的全覆盖测试</td>
</tr>
<tr class="even">
<td><ol start="8" type="1">
<li></li>
</ol></td>
<td>资产被动识别</td>
<td>通过62款型号资产被动识别的全覆盖测试</td>
</tr>
<tr class="odd">
<td><ol start="9" type="1">
<li></li>
</ol></td>
<td>资产主动识别</td>
<td>通过82款资产的主动识别功能全覆盖测试；同时通过19种服务识别功能的全覆盖测试</td>
</tr>
<tr class="even">
<td><ol start="10" type="1">
<li></li>
</ol></td>
<td>漏洞映射</td>
<td>通过xx款资产的xx条漏洞映射全覆盖测试</td>
</tr>
</tbody>
</table>

备注：功能全覆盖测试，不包含稳定性重点测试和发散（S）/探索测试重点（E）。

## 健壮性

目前针对ISTP各模块的健壮性质量特性进行了健壮性测试（特别是协议相关模块）。为确保ISTP各模块的健壮性符合标准，在测试过程中利用Fuzzing测试技术来构造有针对性的异常输入数据。

目前ISTP通过了绿盟漏扫、中京漏挖、博智漏挖等多款产品在OPC
UA、FINS、DNP3、CIP等协议模块的Fuzzing测试，~~测试未发现dp挂死等阻断性问题，符合健壮性发布标准~~，涉及的协议如下表所示。

<table style="width:100%;">
<colgroup>
<col style="width: 10%" />
<col style="width: 23%" />
<col style="width: 13%" />
<col style="width: 13%" />
<col style="width: 13%" />
<col style="width: 24%" />
</colgroup>
<thead>
<tr class="header">
<th>序号</th>
<th>协议</th>
<th>绿盟漏扫</th>
<th>中京漏挖</th>
<th>博智漏挖</th>
<th>备注</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><ol type="1">
<li></li>
</ol></td>
<td>BACnet</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="2" type="1">
<li></li>
</ol></td>
<td>CIP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="3" type="1">
<li></li>
</ol></td>
<td>DNP3-TCP</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="4" type="1">
<li></li>
</ol></td>
<td>DNP3-UDP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="5" type="1">
<li></li>
</ol></td>
<td>Ethernet/IP-TCP</td>
<td></td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="6" type="1">
<li></li>
</ol></td>
<td>Ethernet/IP-UDP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="7" type="1">
<li></li>
</ol></td>
<td>FINS-TCP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="8" type="1">
<li></li>
</ol></td>
<td>FINS-UDP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="9" type="1">
<li></li>
</ol></td>
<td>GOOSE</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="10" type="1">
<li></li>
</ol></td>
<td>IEC104</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="11" type="1">
<li></li>
</ol></td>
<td>MMS</td>
<td></td>
<td><strong>√</strong></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="12" type="1">
<li></li>
</ol></td>
<td>Modbus TCP</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="13" type="1">
<li></li>
</ol></td>
<td>OPC UA</td>
<td></td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="14" type="1">
<li></li>
</ol></td>
<td>Profinet DCP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="15" type="1">
<li></li>
</ol></td>
<td>Profinet MRP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="16" type="1">
<li></li>
</ol></td>
<td>S7</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
</tr>
<tr class="odd">
<td><ol start="17" type="1">
<li></li>
</ol></td>
<td>SV</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
<tr class="even">
<td><ol start="18" type="1">
<li></li>
</ol></td>
<td>HartIP</td>
<td></td>
<td></td>
<td>√</td>
<td></td>
</tr>
</tbody>
</table>

## 稳定性

目前针对ISTP各模块的稳定性质量特性进行了长期稳定测试（特别是协议相关模块），在为期xx天/周的长期测试下，内存占用率约xx、cpu占用率约为xx，丢包率约为xx

## 产品兼容性

目前ISTP各模块已合入工业防火墙、IETC、ISD、漏扫等xx款产品，且已通过工业防火墙、IETC、ISD、漏扫等产品的联合测试，~~未出现dp挂死等阻碍功能使用的问题~~
