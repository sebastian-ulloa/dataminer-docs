---
uid: GetMaskedAlarmsForViewV2
---

# GetMaskedAlarmsForViewV2

Use this method to retrieve the list of all the masked alarms of a particular view, as well as the alarm cache status.

Available from DataMiner 10.0.7 onwards.

## Input

| Item       | Format  | Description                                                                      |
|------------|---------|----------------------------------------------------------------------------------|
| Connection | String  | The connection ID. See [ConnectApp](xref:ConnectApp) . |
| ViewID     | Integer | The view ID.                                                                     |

## Output

| Item                            | Format                                                                   | Description                                                                                 |
|---------------------------------|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| GetMaskedAlarmsFor­ViewV2Result | Array of DMAAlarm (see [DMAAlarm](xref:DMAAlarm)) | The list of all the masked alarms of the specified view, as well as the alarm cache status. |
