# Microsoft.ApiManagement/service/products/groups template reference
API Version: 2017-03-01
## Template format

To create a Microsoft.ApiManagement/service/products/groups resource, add the following JSON to the resources section of your template.

```json
{
  "name": "string",
  "type": "Microsoft.ApiManagement/service/products/groups",
  "apiVersion": "2017-03-01"
}
```
## Property values

The following tables describe the values you need to set in the schema.

<a id="Microsoft.ApiManagement/service/products/groups" />
### Microsoft.ApiManagement/service/products/groups object
|  Name | Type | Required | Value |
|  ---- | ---- | ---- | ---- |
|  name | string | Yes | Group identifier. Must be unique in the current API Management service instance. |
|  type | enum | Yes | Microsoft.ApiManagement/service/products/groups |
|  apiVersion | enum | Yes | 2017-03-01 |

