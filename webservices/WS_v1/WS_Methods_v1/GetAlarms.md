---
uid: GetAlarms
---

# GetAlarms

Use this method to retrieve alarms matching a DMAAlarmFilterV2 object. (Available from DataMiner 9.5.6 onwards.)

## Input

| Item             | Format | Description                                                                                                  |
|------------------|--------|--------------------------------------------------------------------------------------------------------------|
| Connection       | String | The connection ID. See [ConnectApp](xref:ConnectApp).                                                         |
| DMAAlarmFilterV2 | Array  | The filter that the alarms must match. See [DMAAlarmFilterV2](xref:DMAAlarmFilterV2). |

## Output

| Item | Format | Description |
|--|--|--|
| GetAlarmsResult | Array of [DMAAlarm](xref:DMAAlarm) | The alarms matching the specified filter object. |