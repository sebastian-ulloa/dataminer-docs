---
uid: GetResources
---

# GetResources

Use this method to retrieve all resources in the DataMiner System.

## Input

| Item       | Format | Description                                                                          |
|------------|--------|--------------------------------------------------------------------------------------|
| Connection | String | The connection string. See [ConnectApp](xref:ConnectApp) . |

## Output

| Item               | Format                                                                            | Description                            |
|--------------------|-----------------------------------------------------------------------------------|----------------------------------------|
| GetResourcesResult | Array of DMAResource (see [DMAResource](xref:DMAResource)) | The resources in the DataMiner System. |
