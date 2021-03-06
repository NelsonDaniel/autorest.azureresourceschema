# Microsoft.Web/sites/slots/hybridconnection template reference
API Version: 2016-08-01
## Template format

To create a Microsoft.Web/sites/slots/hybridconnection resource, add the following JSON to the resources section of your template.

```json
{
  "name": "string",
  "type": "Microsoft.Web/sites/slots/hybridconnection",
  "apiVersion": "2016-08-01",
  "kind": "string",
  "properties": {
    "entityName": "string",
    "entityConnectionString": "string",
    "resourceType": "string",
    "resourceConnectionString": "string",
    "hostname": "string",
    "port": "integer",
    "biztalkUri": "string"
  }
}
```
## Property values

The following tables describe the values you need to set in the schema.

<a id="Microsoft.Web/sites/slots/hybridconnection" />
### Microsoft.Web/sites/slots/hybridconnection object
|  Name | Type | Required | Value |
|  ---- | ---- | ---- | ---- |
|  name | string | Yes |  |
|  type | enum | Yes | Microsoft.Web/sites/slots/hybridconnection |
|  apiVersion | enum | Yes | 2016-08-01 |
|  kind | string | No | Kind of resource. |
|  properties | object | Yes | RelayServiceConnectionEntity resource specific properties - [RelayServiceConnectionEntityProperties object](#RelayServiceConnectionEntityProperties) |


<a id="RelayServiceConnectionEntityProperties" />
### RelayServiceConnectionEntityProperties object
|  Name | Type | Required | Value |
|  ---- | ---- | ---- | ---- |
|  entityName | string | No |  |
|  entityConnectionString | string | No |  |
|  resourceType | string | No |  |
|  resourceConnectionString | string | No |  |
|  hostname | string | No |  |
|  port | integer | No |  |
|  biztalkUri | string | No |  |

