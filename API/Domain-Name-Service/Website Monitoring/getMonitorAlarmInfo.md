# getMonitorAlarmInfo


## 描述
主域名的监控项的报警信息

## 请求方式
GET

## 请求地址
https://clouddnsservice.jdcloud-api.com/v1/regions/{regionId}/domain/{domainId}/monitor/alarminfo

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**domainId**|String|True||域名ID|
|**regionId**|String|True||Region ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**pageIndex**|Integer|False||当前页数，起始值为1，默认为1|
|**pageSize**|Integer|False||分页查询时设置的每页行数|
|**searchValue**|String|False||关键字|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String||
|**result**|[Result](##Result)||


### <a name="Result">Result</a>
|名称|类型|描述|
|---|---|---|
|**currentCount**|Integer||
|**dataList**|[MonitorAlarmInfo[]](##MonitorAlarmInfo)||
|**totalCount**|Integer||
|**totalPage**|Integer||
### <a name="MonitorAlarmInfo">MonitorAlarmInfo</a>
|名称|类型|描述|
|---|---|---|
|**domainId**|Integer|域名ID|
|**host**|String|故障IP/域名|
|**id**|Integer||
|**startTime**|Integer|故障开始时间|
|**subDomainName**|String|子域名|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|BAD_REQUEST|
