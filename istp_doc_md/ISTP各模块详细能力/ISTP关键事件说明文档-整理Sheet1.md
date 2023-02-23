
# 关键事件-协议

## DNP3

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|DNP3|2|DNP3_EVENT_COLDRST|Cold Restart，冷再启动|event||
||3|DNP3_EVENT_WARMRST|Warm Restart，暖再启动|event||
||4|DNP3_EVENT_SAVECFG|Save Cfg，保存配置|event||
||5|DNP3_EVENT_DELETEFILE|Delete File，删除文件|event||
||6|DNP3_EVENT_INITDATA|Init Data，恢复出厂设置|event||
||7|DNP3_EVENT_INITAPP|Init App，初始化应用程序|event||
||8|DNP3_EVENT_STARTAPP|Start App，启动应用程序|event||
||9|DNP3_EVENT_STOPAPP|Stop App，停止应用程序|event||
||10|DNP3_EVENT_OPENFILE|Open File，打开文件|event||
||11|DNP3_EVENT_CLOSEFILE|Close File，关闭文件|event||
||12|DNP3_EVENT_GETFILEINF|Get File Info，获取文件信息|event||
||13|DNP3_EVENT_AUTHFILE|Auth File，文件认证|event||
||14|DNP3_EVENT_ABORTFILE|Abort File，文件传输中止|event||
||15|DNP3_EVENT_AUTHREQ|Auth Request，身份认证请求|event||
||16|DNP3_EVENT_AUTHERR|Auth Error，身份认证失败通知|event||
||17|DNP3_EVENT_AUTHRESP|Auth Response，身份认证响应|event||
||无|无|Select，选择或打开输出点|info|info类型目前不做为关键事件|
||无|无|Operate，操作选择的输出点|info||
||无|无|Direct Operate(ACK)，直接操作，有响应|info||
||无|无|Direct Operate(NoACK)，直接操作，无响应|info||

## melsec

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|melsec|1|MELSEC_EVENT_PLC_RUN|远程运行。|event||
||2|MELSEC_EVENT_PLC_STOP|远程停止。|event||
||3|MELSEC_EVENT_PLC_PAUSE|远程暂停。|event||
||4|MELSEC_EVENT_PLC_CLEAR_LATCH|远程锁存清除。|event||
||5|MELSEC_EVENT_PLC_RESET|远程重置。|event||
||6|MELSEC_EVENT_PLC_LOCK|远程锁。|event||
||7|MELSEC_EVENT_PLC_UNLOCK|远程解锁。|event||
||8|MELSEC_EVENT_PLC_CLEAR_ERROR|错误信息清除。|event||
||9|MELSEC_EVENT_PLC_CREATE|新建文件|event||
||10|MELSEC_EVENT_PLC_REMOVE|删除文件|event||
||11|MELSEC_EVENT_PLC_COPY|复制文件|event||
||12|MELSEC_EVENT_PLC_ATTR_ALTER|文件属性修改|event||
||13|MELSEC_EVENT_PLC_DATE_ALTER|文件创建时间修改|event||
||14|MELSEC_EVENT_PLC_OPEN|打开文件|event||
||15|MELSEC_EVENT_PLC_READ|读文件|event||
||16|MELSEC_EVENT_PLC_WRITE|写文件|event||
||17|MELSEC_EVENT_PLC_CLOSE|关闭文件|event||
||18|MELSEC_EVENT_PLC_BUF_WRITE|写缓冲存储器。|event||
||19|MELSEC_EVENT_PLC_BUF_MODULE_WRITE|写智能模块缓冲存储器。|event||

## mms

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|mms 61850|1|mms_EVENT_rename|rename|event||
||2|mms_EVENT_write|write|event||
||3|mms_EVENT_defineNamedVariable|defineNamedVariable|event||
||4|mms_EVENT_defineScatteredAccess|defineScatteredAccess|event||
||5|mms_EVENT_deleteVariableAccess|deleteVariableAccess|event||
||6|mms_EVENT_defineNamedVariableList|defineNamedVariableList|event||
||7|mms_EVENT_deleteNamedVariableList|deleteNamedVariableList|event||
||8|mms_EVENT_defineNamedType|defineNamedType|event||
||9|mms_EVENT_deleteNamedType|deleteNamedType|event||
||10|mms_EVENT_input|input|event||
||11|mms_EVENT_output|output|event||
||12|mms_EVENT_takeControl|takeControl|event||
||13|mms_EVENT_relinquishControl|relinquishControl|event||
||14|mms_EVENT_defineSemaphore|defineSemaphore|event||
||15|mms_EVENT_deleteSemaphore|deleteSemaphore|event||
||16|mms_EVENT_initiateDownloadSequence|initiateDownloadSequence|event||
||17|mms_EVENT_downloadSegment|downloadSegment|event||
||18|mms_EVENT_terminateDownloadSequence|terminateDownloadSequence|event||
||19|mms_EVENT_initiateUploadSequence|initiateUploadSequence|event||
||20|mms_EVENT_uploadSegment|uploadSegment|event||
||21|mms_EVENT_terminateUploadSequence|terminateUploadSequence|event||
||22|mms_EVENT_requestDomainDownload|requestDomainDownload|event||
||23|mms_EVENT_requestDomainUpload|requestDomainUpload|event||
||24|mms_EVENT_loadDomainContent|loadDomainContent|event||
||25|mms_EVENT_storeDomainContent|storeDomainContent|event||
||26|mms_EVENT_deleteDomain|deleteDomain|event||
||27|mms_EVENT_createProgramInvocation|createProgramInvocation|event||
||28|mms_EVENT_deleteProgramInvocation|deleteProgramInvocation|event||
||29|mms_EVENT_start|start|event||
||30|mms_EVENT_stop|stop|event||
||31|mms_EVENT_resume|resume|event||
||32|mms_EVENT_reset|reset|event||
||33|mms_EVENT_kill|kill|event||
||34|mms_EVENT_obtainFile|obtainFile|event||
||35|mms_EVENT_defineEventCondition|defineEventCondition|event||
||36|mms_EVENT_deleteEventCondition|deleteEventCondition|event||
||37|mms_EVENT_alterEventConditionMonitoring|alterEventConditionMonitoring|event||
||38|mms_EVENT_triggerEvent|triggerEvent|event||
||39|mms_EVENT_defineEventAction|defineEventAction|event||
||40|mms_EVENT_deleteEventAction|deleteEventAction|event||
||41|mms_EVENT_defineEventEnrollment|defineEventEnrollment|event||
||42|mms_EVENT_deleteEventEnrollment|deleteEventEnrollment|event||
||43|mms_EVENT_alterEventEnrollment|alterEventEnrollment|event||
||44|mms_EVENT_writeJournal|writeJournal|event||
||45|mms_EVENT_initializeJournal|initializeJournal|event||
||46|mms_EVENT_createJournal|createJournal|event||
||47|mms_EVENT_deleteJournal|deleteJournal|event||
||48|mms_EVENT_fileRename|fileRename|event||
||49|mms_EVENT_fileDelete|fileDelete|event||
||50|mms_EVENT_fileOpen|fileOpen|event||
||51|mms_EVENT_fileRead|fileRead|event||
||52|mms_EVENT_fileClose|fileClose|event||

## bacnet

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|BACnet|1|BACNET_EVENT_Write_Broadcast_Distribution_Table|Write-Broadcast-Distribution-Table,写广播分发表。|info||
||2|BACNET_EVENT_Register_Foreign_Device|Register-Foreign-Device，注册外部设备。|event||
||3|BACNET_EVENT_Delete_Foreign_Device_Table_Entry|Delete-Foreign-Device-Table-Entry，从表中删除外部设备。|event||
||4|BACNET_EVENT_Distribute_Broadcast_To_Network|Distribute-Broadcast-To-Network，此消息提供一种机制：外部设备可以使BBMD在所有IP子网上广播消息。|event||

## coap

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|Coap|1|COAP_EVENT_RESPONSE_BAD_REQUEST|Bad Request,请求错误，服务器无法处理。类似于HTTP 400。|event||
||2|COAP_EVENT_RESPONSE_UNAUTHORIZED|Unauthorized，没有权限。类似于HTTP 401。|event||
||3|COAP_EVENT_RESPONSE_BAD_OPTION|Bad Option，请求中包含错误选项|event||
||4|COAP_EVENT_RESPONSE_FORBIDDEN|Forbidden，服务器拒绝请求。类似于HTTP 403。|event||
||5|COAP_EVENT_RESPONSE_NOT_FOUND|Not Found，服务器找不到资源。类似于HTTP 404。|event||
||6|COAP_EVENT_RESPONSE_METHOD_NOT_ALLOWED|Method Not Allowed，非法请求方法。类似于HTTP 405。|event||
||7|COAP_EVENT_RESPONSE_NOT_ACCEPTABLE|Not Acceptable，请求选项和服务器生成的内容选项不一致。类似于HTTP 406。|event||
||8|COAP_EVENT_RESPONSE_PRECONDITION_FAILDED|Precondition Failed，请求参数不足。类似于HTTP 412。|event||
||9|COAP_EVENT_RESPONSE_UNSUPPOR_CONTEN_TYPE|Unsuppor Conten-Type，请求中的媒体类型不足。类似于HTTP 415。|event||
||10|COAP_EVENT_RESPONSE_INTERNAL_SERVER_ERROR|Internal Server Error，服务器内部错误，类似于HTTP 500。|event||
||11|COAP_EVENT_RESPONSE_NOT_IMPLEMENTED|Not Implemented，服务器无法支持请求内容。类似于HTTP 501。|event||
||12|COAP_EVENT_RESPONSE_BAD_GATEWAY|Bad Gateway，服务器作为网关时，收到一个错误的响应。类似于HTTP 502。|event||
||13|COAP_EVENT_RESPONSE_SERVICE_UNAVAILABE|Service Unavailable，服务器过载或者维护停机。类似于HTTP 503。|event||
||14|COAP_EVENT_RESPONSE_GATEWAY_TIMEOUT|Gateway Timeout，服务器作为网关时，执行请求时发送超时错误。类似于HTTP 504。|event||
||15|COAP_EVENT_RESPONSE_PROXY_NOT_SUPPORTED|Proxying Not Supported，服务器不支持代理功能。|event||

## ENIP_CIP

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|enip cip Common|1|ENIP_CIP_EVENT_SC_SET_ATT_ALL|SET_ATT_ALL|info||
||2|ENIP_CIP_EVENT_SC_SET_ATT_LIST|SET_ATT_LIST|info||
||3|ENIP_CIP_EVENT_SC_RESET|RESET|event||
||4|ENIP_CIP_EVENT_SC_START|START|event||
||5|ENIP_CIP_EVENT_SC_STOP|STOP|event||
||6|ENIP_CIP_EVENT_SC_CREATE|CREATE|event||
||7|ENIP_CIP_EVENT_SC_DELETE|DELETE|event||
||8|ENIP_CIP_EVENT_SC_APPLY_ATTRIBUTES|APPLY_ATTRIBUTES|event||
||9|ENIP_CIP_EVENT_SC_SET_ATT_SINGLE|SET_ATT_SINGLE|info||
||10|ENIP_CIP_EVENT_SC_RESTOR|RESTOR|event||
||11|ENIP_CIP_EVENT_SC_SAVE|SAVE|event||
||12|ENIP_CIP_EVENT_SC_SET_MEMBER|SET_MEMBER|info||
||13|ENIP_CIP_EVENT_SC_INSERT_MEMBER|INSERT_MEMBER|event||
||14|ENIP_CIP_EVENT_SC_REMOVE_MEMBER|REMOVE_MEMBER|event||
||15|ENIP_CIP_EVENT_SC_DOWNLOAD|DOWNLOAD|event||
||16|ENIP_CIP_EVENT_SC_UPLOAD|UPLOAD|event||

## ENIP_CIP_Logix5000

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|enip cip Logix5000|17|ENIP_CIP_LOGIX5000_EVENT_WRITE_DATA|Logix5000 CIP Write Data Service|info||
||18|ENIP_CIP_LOGIX5000_EVENT_WRITE_DATA_FRAGMENTED_FORMAT|Logix5000 Write Data Fragmented Format Service|info||

## ENIP_CIP_PCCC

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|enip cip pccc|19|ENIP_CIP_PCCC_EVENT_BIT_WRITE|bit write|info||
||20|ENIP_CIP_PCCC_EVENT_DOWNLOAD_ALL_REQUEST|download all request|event||
||21|ENIP_CIP_PCCC_EVENT_DOWNLOAD_COMPLETED|download completed|event||
||22|ENIP_CIP_PCCC_EVENT_DOWNLOAD_REQUEST|download request|event||
||23|ENIP_CIP_PCCC_EVENT_FILE_WRITE|file write|event||
||24|ENIP_CIP_PCCC_EVENT_PHYSICAL_WRITE|physical write|info||
||25|ENIP_CIP_PCCC_EVENT_PHYSICAL_BIT_WRITE|protected bit write|info||
||26|ENIP_CIP_PCCC_EVENT_PROTECTED_TYPED_FILE_WRITE|protected typed file write|info||
||27|ENIP_CIP_PCCC_EVENT_PROTECTED_TYPED_LOGICAL_WRITE|protected typed logical write|info||
||28|ENIP_CIP_PCCC_EVENT_PROTECTED_WRITE|protected write|info||
||29|ENIP_CIP_PCCC_EVENT_RESTART_REQUEST|restart request|event||
||30|ENIP_CIP_PCCC_EVENT_SET_CPU_MODE|set CPU mode|event||
||31|ENIP_CIP_PCCC_EVENT_SHUTDOWN|shutdown|event||
||32|ENIP_CIP_PCCC_EVENT_TYPED_WRITE|typed write|info||
||33|ENIP_CIP_PCCC_EVENT_UNPORTECTED_BIT_WRITE|unprotected bit write|info||
||34|ENIP_CIP_PCCC_EVENT_UNPORTECTED_WRITE|unprotected write|info||
||35|ENIP_CIP_PCCC_EVENT_UPLOAD_ALL_REQUEST|upload all request (upload)|event||
||36|ENIP_CIP_PCCC_EVENT_UPLOAD_COMPLETED|upload completed|event||
||37|ENIP_CIP_PCCC_EVENT_UPLOAD|upload|event||
||38|ENIP_CIP_PCCC_EVENT_WORD_RANGE_WRITE|word range write|info||
||39|ENIP_CIP_PCCC_EVENT_WRITE_BYTES_PHYSICAL|write bytes physical|info||

## Etrol_SL304

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|Etrol SL304|1|ETROL_SL304_TCP_WELLHEAD_CONFIG_WRITE|WELLHEAD_CONFIG_WRITE|event||
||2|ETROL_SL304_TCP_RTU_CONFIG_WRITE_PARAMETER|RTU_CONFIG_WRITE_PARAMETER|event||
||3|ETROL_SL304_TCP_BOOT_UP|BOOT_UP|event||
||4|ETROL_SL304_TCP_SHUT_DOWN|SHUT_DOWN|event||
||5|ETROL_SL304_TCP_AI_MEASURE_RANGE_WRITE|AI_MEASURE_RANGE_WRITE|event||
||6|ETROL_SL304_TCP_INSTRUMENT_ALARM|INSTRUMENT_ALARM|event||

## Focas

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|Focas|1|FOCAS_EVENT_SETUP_CONNECTION|SETUP_CONNECTION|event||
||2|FOCAS_EVENT_START|START|event||
||3|FOCAS_EVENT_STOP|STOP|event||

## FX

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|fx|无|无|无|||

## GDW3761

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|gdw3761|1|GDW3761_EVENT_RSET|复位|event||
||2|GDW3761_EVENT_AUTH|身份认证及密钥协商|event||

## Goose

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|Goose|1|GOOSE_EVENT_TestStatus|TestStatus|event||

## HartIP

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|HartIP|1|HARTIP_EVENT_WRITE_MSG|写信息|event||
||2|HARTIP_EVENT_WRITE_TAG|写短标签、设备描述符和日期|event||
||3|HARTIP_EVENT_WRITE_NUMBER|写最终装配号|event||
||4|HARTIP_EVENT_WRITE_LONG_TAG|写长标签|event||
||5|HARTIP_EVENT_RESET_CONFIG_CHANGR_FLAG|复位配置改变标志|event||

## ht_2000r_tcp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|ht_2000r_tcp|1|HT_2000R_TCP_OILWELL_START|OILWELL_START|event||
||2|HT_2000R_TCP_OILWELL_STOP|OILWELL_STOP|event||
||3|HT_2000R_TCP_BURNER_IGNITE|BURNER_IGNITE|event||
||4|HT_2000R_TCP_BURNER_TURNOFF|BURNER_TURNOFF|event||
||5|HT_2000R_TCP_ELECTRIC_BRAKE_LOCK|ELECTRIC_BRAKE_LOCK|event||
||6|HT_2000R_TCP_ELECTRIC_BRAKE_LOOSEN|ELECTRIC_BRAKE_LOOSEN|event||
||7|HT_2000R_TCP_BALANCE_ADJUSTMENT_START|BALANCE_ADJUSTMENT_START|event||
||8|HT_2000R_TCP_BALANCE_ADJUSTMENT_STOP|BALANCE_ADJUSTMENT_STOP|event||
||9|HT_2000R_TCP_RTU_RESET|RTU_RESET|event||

## IEC104

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|IEC104|1|IEC104_EVENT_C_SC_NA_1|single command|event||
||2|IEC104_EVENT_C_SC_TA_1|single command with time tag CP56Time2a|event||
||3|IEC104_EVENT_C_DC_NA_1|double command|event||
||4|IEC104_EVENT_C_DC_TA_1|double command with time tag CP56Time2a|event||
||5|IEC104_EVENT_C_RC_NA_1|regulating step command|event||
||6|IEC104_EVENT_C_RC_TA_1|regulating step command with time tag CP56Time2a|event||
||7|IEC104_EVENT_C_SE_NA_1|set point command, normalized value|info||
||8|IEC104_EVENT_C_SE_TA_1|set point command, normalized value with time tag CP56Time2a|event||
||9|IEC104_EVENT_C_SE_NB_1|set point command, scaled value|event||
||10|IEC104_EVENT_C_SE_TB_1|set point command, scaled value with time tag CP56Time2a|event||
||11|IEC104_EVENT_C_SE_NC_1|set point command, short floating point number|event||
||12|IEC104_EVENT_C_SE_TC_1|set point command, short floating-point number with time tag CP56Time2a|event||
||13|IEC104_EVENT_C_BO_NA_1|bitstring of 32 bits|event||
||14|IEC104_EVENT_C_BO_TA_1|bitstring of 32 bits with time tag CP56Time2a|info||
||15|IEC104_EVENT_C_RP_NA_1|reset process command|event||

## JX300

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|JX300|1|JX300_EVENT_SEND_DEVICE_INFO|SEND_DEVICE_INFO|event||
||2|JX300_EVENT_SET_DEVICE_VALUE|SET_DEVICE_VALUE|event||
||3|JX300_EVENT_SET_DEVICE_STATE|SET_DEVICE_STATE|event||

## Modbus

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|Modbus|1|MODBUS_EVENT_WRITE_SINGLE_COIL|WRITE_SINGLE_COIL|event||
||2|MODBUS_EVENT_WRITE_MULT_COILS|WRITE_MULT_COILS|event||
||3|MODBUS_EVENT_WRITE_SINGLE_REG|WRITE_SINGLE_REG|event||
||4|MODBUS_EVENT_WRITE_MULT_REGS|WRITE_MULT_REGS|event||
||5|MODBUS_EVENT_PLC_START|PLC_START|event||
||6|MODBUS_EVENT_PLC_STOP|PLC_STOP|event||
||7|MODBUS_EVENT_PLC_DOWNLOAD_START|PLC_DOWNLOAD_START|event||
||8|MODBUS_EVENT_PLC_DOWNLOAD_END|PLC_DOWNLOAD_END|event||
||9|MODBUS_EVENT_PLC_UPLOAD_START|PLC_UPLOAD_START|event||
||10|MODBUS_EVENT_PLC_UPLOAD_END|PLC_UPLOAD_END|event||
||11|MODBUS_EVENT_PLC_FORCE_1|PLC_FORCE_1|event||
||12|MODBUS_EVENT_PLC_FORCE_0|PLC_FORCE_0|event||
||13|MODBUS_EVENT_PLC_FORCE_CANCEL|PLC_FORCE_CANCEL|event||

## MQTT

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|mqtt|无|无|无|||

## na_rtu_oil_tcp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|na_rtu_oil_tcp|1|NA_RTU_OIL_TCP_RESET|RESET|event||
||2|NA_RTU_OIL_TCP_CLOSE_PROCESS|CLOSE_PROCESS|event||
||3|NA_RTU_OIL_TCP_CLOSE_WATCHDOG|CLOSE_WATCHDOG|event||
||4|NA_RTU_OIL_TCP_RTU_PARAMETER_CONFIG_DOWNLOAD|RTU_PARAMETER_CONFIG_DOWNLOAD|event||
||5|NA_RTU_OIL_TCP_INSTRUMENT_PARAMETER_CONFIG_SET|INSTRUMENT_PARAMETER_CONFIG_SET|event||
||6|NA_RTU_OIL_TCP_STARTUP_WELL|STARTUP_WELL|event||
||7|NA_RTU_OIL_TCP_SHUTDOWN_WELL|SHUTDOWN_WELL|event||
||8|NA_RTU_OIL_TCP_HEATING_FURNACE_IGNITE|HEATING_FURNACE_IGNITE|event||
||9|NA_RTU_OIL_TCP_HEATING_FURNACE_TURNOFF|HEATING_FURNACE_TURNOFF|event||
||10|NA_RTU_OIL_TCP_OIL_WELL_FREQUENCY_SET|OIL_WELL_FREQUENCY_SET|event||

## nriec103

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|nriec103|无|无|无|||

## Omron_Fins

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|omron|1|OMRON_EVENT_PLC_RESET|PLC_RESET|event||
||2|OMRON_EVENT_PLC_RUN|PLC_RUN|event||
||3|OMRON_EVENT_PLC_STOP|PLC_STOP|event||
||4|OMRON_EVENT_FORCED_SET_RESET|FORCED_SET_RESET|event||
||5|OMRON_EVENT_CLOCK_WRITE|CLOCK_WRITE|event||
||7|OMRON_EVENT_ACCESS_RIGTH_ACQUIRE|ACCESS_RIGTH_ACQUIRE|event||
||9|OMRON_EVENT_PLC_SINGLE_FILE_WRITE|PLC_SINGLE_FILE_WRITE|event||
||10|OMRON_EVENT_FORCED_SET_RESET_CANCEL|FORCED_SET_RESET_CANCEL|event||
||11|OMRON_EVENT_PLC_ERROR_CLEAR|PLC_ERROR_CLEAR|event||
||12|OMRON_EVENT_PLC_ERROR_LOG_CLEAR|PLC_ERROR_LOG_CLEAR|event||
||13|OMRON_EVENT_ACCESS_RIGHT_FORCED_ACQUIRE|ACCESS_RIGHT_FORCED_ACQUIRE|event||
||14|OMRON_EVENT_FILE_DELETE|FILE_DELETE|event||
||15|OMRON_EVENT_MEMORY_WRITE|MEMORY_WRITE|event||
||16|OMRON_EVENT_MEMORY_FILL|MEMORY_FILL|event||
||17|OMRON_EVENT_PROGRAM_WRITE|PROGRAM_WRITE|event||
||18|OMRON_EVENT_PROGRAM_CLEAR|PROGRAM_CLEAR|event||
||19|OMRON_EVENT_PARAMETER_PROTECT_CLEAR|PARAMETER_PROTECT_CLEAR|event||
||20|OMRON_EVENT_PARAMETER_AREA_CLEAR|PARAMETER_AREA_CLEAR|event||
||21|OMRON_EVENT_PROGRAM_AREA_PROTECT|PROGRAM_AREA_PROTECT|event||
||22|OMRON_EVENT_MESSAGE_CLEAR|MESSAGE_CLEAR|event||
||23|OMRON_EVENT_FILE_COPY|FILE_COPY|event||
||24|OMRON_EVENT_FILE_NAME_CHANGE|FILE_NAME_CHANGE|event||
||25|OMRON_EVENT_MEMORY_AREA_FILE_TRANSFER|MEMORY_AREA_FILE_TRANSFER|event||
||26|OMRON_EVENT_PARAMETER_AREA_FILE_TRANSFER|PARAMETER_AREA_FILE_TRANSFER|event||
||27|OMRON_EVENT_PROGRAM_AREA_FILE_TRANSFER|PROGRAM_AREA_FILE_TRANSFER|event||

## OPC_DA

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|opcda|1|OPCDA_EVENT_IOPCITEMIO_WRITEVQT|为指定的Item写一个或多个值、质量和时间戳。|info||
||2|OPCDA_EVENT_IOPCSYNCIO_WRITE|以同步方式将值写入OPCGroup內的OPCItem(s)|info||
||3|OPCDA_EVENT_IOPCSYNCIO2_WRITE|以同步方式将值写入OPCGroup內的OPCItem(s)|info||
||4|OPCDA_EVENT_IOPCSYNCIO2_WRITEVQT|设置多个指定的Item的值、质量和时间戳。|info||
||5|OPCDA_EVENT_IOPCASYNCIO_WRITE|以非同步方式将值写入OPCGroup内的OPCItem(s)|info||
||6|OPCDA_EVENT_IOPCASYNCIO2_WRITE|以非同步方式将值写入OPCGroup内的OPCItem(s)|info||
||7|OPCDA_EVENT_IOPCASYNCIO3_WRITE|以非同步方式将值写入OPCGroup内的OPCItem(s)|info||
||8|OPCDA_EVENT_IOPCASYNCIO3_WRITEVQT|设置多个指定的Item的值、质量和时间戳。|info||
||9|OPCDA_EVENT_IOPCSHUTDOWN_SHUTDOWNREQ|断开连接请求|info||

## OPC_UA

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|opcua|1|OPCUA_EVENT_ServiceFault|ServiceFault|event||
||2|OPCUA_EVENT_RegisterServerRequest|RegisterServerRequest|event||
||3|OPCUA_EVENT_CloseSecureChannelRequest|CloseSecureChannelRequest|event||
||4|OPCUA_EVENT_CreateSessionRequest|CreateSessionRequest|event||
||5|OPCUA_EVENT_ActivateSessionRequest|ActivateSessionRequest|event||
||6|OPCUA_EVENT_CloseSessionRequest|CloseSessionRequest|event||
||7|OPCUA_EVENT_CancelRequest|CancelRequest|event||
||8|OPCUA_EVENT_AddNodesRequest|AddNodesRequest|event||
||9|OPCUA_EVENT_AddReferencesRequest|AddReferencesRequest|event||
||10|OPCUA_EVENT_DeleteNodesRequest|DeleteNodesRequest|event||
||11|OPCUA_EVENT_DeleteReferencesRequest|DeleteReferencesRequest|event||
||12|OPCUA_EVENT_TranslateBrowsePathsToNodeIdsRequest|TranslateBrowsePathsToNodeIdsRequest|event||
||13|OPCUA_EVENT_RegisterNodesRequest|RegisterNodesRequest|event||
||14|OPCUA_EVENT_UnregisterNodesRequest|UnregisterNodesRequest|event||
||15|OPCUA_EVENT_WriteRequest|WriteRequest|event||
||16|OPCUA_EVENT_HistoryUpdateRequest|HistoryUpdateRequest|event||
||17|OPCUA_EVENT_CallRequest|CallRequest|event||
||18|OPCUA_EVENT_CreateMonitoredItemsRequest|CreateMonitoredItemsRequest|event||
||19|OPCUA_EVENT_ModifyMonitoredItemsRequest|ModifyMonitoredItemsRequest|event||
||20|OPCUA_EVENT_SetMonitoringModeRequest|SetMonitoringModeRequest|event||
||21|OPCUA_EVENT_SetTriggeringRequest|SetTriggeringRequest|event||
||22|OPCUA_EVENT_DeleteMonitoredItemsRequest|DeleteMonitoredItemsRequest|event||
||23|OPCUA_EVENT_CreateSubscriptionRequest|CreateSubscriptionRequest|event||
||24|OPCUA_EVENT_ModifySubscriptionRequest|ModifySubscriptionRequest|event||
||25|OPCUA_EVENT_SetPublishingModeRequest|SetPublishingModeRequest|event||
||26|OPCUA_EVENT_PublishRequest|PublishRequest|event||
||27|OPCUA_EVENT_RepublishRequest|RepublishRequest|event||
||28|OPCUA_EVENT_TransferSubscriptionsRequest|TransferSubscriptionsRequest|event||
||29|OPCUA_EVENT_DeleteSubscriptionsRequest|DeleteSubscriptionsRequest|event||
||30|OPCUA_EVENT_TestStackRequest|TestStackRequest|event||

## Ovation_TCP

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|ovation tcp|1|TCP_RESTART|TCP_RESTART|event||
||2|TCP_DOWNLOAD|TCP_DOWNLOAD|event||
||3|TCP_LOAD|TCP_LOAD|event||

## Ovation_UDP

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|ovation udp|1|UDP_READ|UDP_READ|info||
||2|UDP_WRITE|UDP_WRITE|info||

## profinet_dcp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_dcp|1|PROFINET_DCP_EVENT_SET_REQUEST|SET_REQUEST|event||

## profinet_mrp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_mrp|4|PROFINET_MRP_EVENT_TOPOLOGYCHANGE,|TOPOLOGYCHANGE|event||
||5|PROFINET_MRP_EVENT_LINKDOWN,|LINKDOWN|event||
||6|PROFINET_MRP_EVENT_LINKUP,|LINKUP|event||

## profinet_mrrt

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_mrrt|1|PROFINET_MRRT_EVENT_END|END|||
||2|PROFINET_MRRT_EVENT_COMMON|COMMON|||
||3|PROFINET_MRRT_EVENT_TEST|TEST|||

## profinet_ptcp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_ptcp|1|PROFINET_PTCP_EVENT_END|END|||
||2|PROFINET_PTCP_EVENT_SUBDOMAIN|SUBDOMAIN|||
||3|PROFINET_PTCP_EVENT_TIME|TIME|||
||4|PROFINET_PTCP_EVENT_TIME_EXTENSION|TIME_EXTENSION|||
||5|PROFINET_PTCP_EVENT_MASTER|MASTER|||
||6|PROFINET_PTCP_EVENT_PORT_PARAMETER|PORT_PARAMETER|||
||7|PROFINET_PTCP_EVENT_DELAY_PARAMETER|DELAY_PARAMETER|||
||8|PROFINET_PTCP_EVENT_PORT_TIME|PORT_TIME|||
||9|PROFINET_PTCP_EVENT_OPTION|OPTION|||

## profinet_rtc1

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_rtc1|无|无|无|||

## profient_rtc3

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|profinet_rtc3|无|无|无|||

## rssp_1

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|rssp_1|1|RSSP_1_TIME_SEQ_REQ|TIME_SEQ_REQ|||

## S7comm

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|s7comm|1|S7COMM_EVENT_FORCES_DI_AI|强制DI/AI|event||
||2|S7COMM_EVENT_REMOVE_DI|删除DI值|event||
||5|S7COMM_EVENT_DIAGNOSTIC|诊断|event||
||6|S7COMM_EVENT_PLC_ERASE|清空PLC内存|event||
||7|S7COMM_EVENT_SET_CLOCK|设置时钟|event||
||8|S7COMM_EVENT_PLC_PASSWD|设置PLC密码|event||
||9|S7COMM_EVENT_DOWNLOAD_BLOCK_REQUEST|请求下载|event||
||10|S7COMM_EVENT_DOWNLOAD_BLOCK_DATA|开始下载|event||
||11|S7COMM_EVENT_DOWNLOAD_BLOCK_END|下载完成|event||
||13|S7COMM_EVENT_UPLOAD_START|开始上载|event||
||14|S7COMM_EVENT_UPLOAD_DATA|上载|event||
||15|S7COMM_EVENT_UPLOAD_END|上载结束|event||
||16|S7COMM_EVENT_PLC_START|PLC启动|event||
||17|S7COMM_EVENT_PLC_STOP|PLC停止|event||
||18|S7COMM_EVENT_MODULE_INSE|激活设备上下载的块|event||
||19|S7COMM_EVENT_MODULE_DEL|从设备的文件系统中删除一个块|event||
||20|S7COMM_EVENT_PLC_GARB|压缩PLC内存|event||
||21|S7COMM_EVENT_PLC_MODU|将RAM复制到ROM|event||
||22|S7COMM_EVENT_WRITE_VAR|写变量|info||
||23|S7COMM_EVENT_WARM_START|暖启动|event||
||24|S7COMM_EVENT_DOWNLOAD_FIREWARE_REQUEST|请求更新固件|event||
||25|S7COMM_EVENT_DOWNLOAD_FIREWARE_DATA|更新固件|event||
||26|S7COMM_EVENT_DOWNLOAD_FIREWARE_END|结束更新固件|event||
||27|S7COMM_EVENT_STOP|停止|event||
||28|S7COMM_EVENT_WARM_RESTART|暖重启|event||
||29|S7COMM_EVENT_RUN|启动|event||
||30|S7COMM_EVENT_HOT_RESTART|热重启|event||
||31|S7COMM_EVENT_COLD_RESTART|冷重启|event||
||32|S7COMM_EVENT_UPDATE|更新|event||

## S7_PLUS

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|s7_plus|1|S7COMM_PLUS_EVENT_DOWNLOAD_START|DOWNLOAD_START|event||
||2|S7COMM_PLUS_EVENT_DOWNLOAD_END|DOWNLOAD_END|event||
||3|S7COMM_PLUS_EVENT_UPLOAD_START|UPLOAD_START|event||
||5|S7COMM_PLUS_EVENT_CPU_START|CPU_START|event||
||6|S7COMM_PLUS_EVENT_CPU_STOP|CPU_STOP|event||
||7|S7COMM_PLUS_EVENT_SYSTEM_TIME|SYSTEM_TIME|event||

## srtp

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|srtp|1|SRTP_EVENT_STOP|stop|||
||2|SRTP_EVENT_START|start|||
||3|SRTP_EVENT_DOWNLOAD|download|||

## sv

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|sv|无|无|无|||

## xhican

|协议名称|Event ID|Event String|含义|事件类型|备注|
|:--|:--|:--|:--|:--|:--|
|xhican|1|XHICAN_EVENT_UPLOAD|UPLOAD|||
||2|XHICAN_EVENT_MOD_PWD|modify password|||
||3|XHICAN_EVENT_CLEAN_CFG|clean configuration|||
||4|XHICAN_EVENT_RESET_CTL|reset controller|||
