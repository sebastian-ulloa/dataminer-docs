---
uid: GetHistoryAlarmsForElement
---

# GetHistoryAlarmsForElement

Use this method in order to retrieve the history alarms for a particular element.

Available from DataMiner version 9.5.1 onwards.

## Input

| Item | Format | Description |
|--|--|--|
| connection | String | The connection ID. See [ConnectApp](xref:ConnectApp). |
| dmaID | Integer | The DataMiner Agent ID. |
| elementID | Integer | The element ID. |
| utcStartTime | Long integer | The start time of the timespan for which alarms should be retrieved, in UTC format (milliseconds since midnight January 1, 1970 GMT). |
| utcEndTime | Long integer | The end time of the timespan for which alarms should be retrieved, in UTC format (milliseconds since midnight January 1, 1970 GMT). |
| filter | Array | Array of filters limiting which alarms will be retrieved. |
| filter.IncludeInforma­tionEvents | Boolean | When true, information events will also be included. |
| filter.IncludeEntire­AlarmTree | Boolean | When true, all alarms are included. Otherwise, only the top alarms of every alarm tree are returned. |
| filter.AlarmTypes | Array of string | Only alarms with an alarm type specified in this array will be returned (default: null). |
| filter.Severities | Array of string | Only alarms with a severity specified in this array will be returned (default: null). |

## Output

| Item | Format | Description |
|--|--|--|
| GetHistoryAlarms­ForElementResult | Array of [DMAAlarm](xref:DMAAlarm) | The alarms for the specified element and period, limited by the specified filters. |
