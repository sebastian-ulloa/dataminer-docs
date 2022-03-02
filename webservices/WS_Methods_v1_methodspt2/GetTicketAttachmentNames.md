---
uid: GetTicketAttachmentNames
---

# GetTicketAttachmentNames

Use this method to retrieve the names of all files attached to a specific ticket. Available from DataMiner 10.0.10 onwards.

> [!NOTE]
> DataMiner Ticketing requires a Cassandra database as well as a specific license. From DataMiner 10.0.13 onwards, it also requires DataMiner Indexing. For more information on acquiring a Ticketing license, contact the Skyline Sales department.

## Input

| Item       | Format  | Description                                                                      |
|------------|---------|----------------------------------------------------------------------------------|
| Connection | String  | The connection ID. See [ConnectApp](xref:ConnectApp) . |
| DmaID      | Integer | The DataMiner Agent ID.                                                          |
| TicketID   | Integer | The ticket ID.                                                                   |

## Output

| Item                            | Format          | Description                                           |
|---------------------------------|-----------------|-------------------------------------------------------|
| GetTicketAttachment­NamesResult | Array of string | The names of the attachments of the specified ticket. |
