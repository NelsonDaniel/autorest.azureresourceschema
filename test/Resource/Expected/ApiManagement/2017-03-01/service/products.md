# Microsoft.ApiManagement/service/products template reference
API Version: 2017-03-01
## Template format

To create a Microsoft.ApiManagement/service/products resource, add the following JSON to the resources section of your template.

```json
{
  "name": "string",
  "type": "Microsoft.ApiManagement/service/products",
  "apiVersion": "2017-03-01",
  "properties": {
    "description": "string",
    "terms": "string",
    "subscriptionRequired": boolean,
    "approvalRequired": boolean,
    "subscriptionsLimit": "integer",
    "state": "string",
    "displayName": "string"
  },
  "resources": []
}
```
## Property values

The following tables describe the values you need to set in the schema.

<a id="Microsoft.ApiManagement/service/products" />
### Microsoft.ApiManagement/service/products object
|  Name | Type | Required | Value |
|  ---- | ---- | ---- | ---- |
|  name | string | Yes | Product identifier. Must be unique in the current API Management service instance. |
|  type | enum | Yes | Microsoft.ApiManagement/service/products |
|  apiVersion | enum | Yes | 2017-03-01 |
|  properties | object | Yes | Product entity contract properties. - [ProductContractProperties object](#ProductContractProperties) |
|  resources | array | No | [policies](./products/policies.md) [groups](./products/groups.md) [apis](./products/apis.md) |


<a id="ProductContractProperties" />
### ProductContractProperties object
|  Name | Type | Required | Value |
|  ---- | ---- | ---- | ---- |
|  description | string | No | Product description. May include HTML formatting tags. |
|  terms | string | No | Product terms of use. Developers trying to subscribe to the product will be presented and required to accept these terms before they can complete the subscription process. |
|  subscriptionRequired | boolean | No | Whether a product subscription is required for accessing APIs included in this product. If true, the product is referred to as "protected" and a valid subscription key is required for a request to an API included in the product to succeed. If false, the product is referred to as "open" and requests to an API included in the product can be made without a subscription key. If property is omitted when creating a new product it's value is assumed to be true. |
|  approvalRequired | boolean | No | whether subscription approval is required. If false, new subscriptions will be approved automatically enabling developers to call the product’s APIs immediately after subscribing. If true, administrators must manually approve the subscription before the developer can any of the product’s APIs. Can be present only if subscriptionRequired property is present and has a value of false. |
|  subscriptionsLimit | integer | No | Whether the number of subscriptions a user can have to this product at the same time. Set to null or omit to allow unlimited per user subscriptions. Can be present only if subscriptionRequired property is present and has a value of false. |
|  state | enum | No | whether product is published or not. Published products are discoverable by users of developer portal. Non published products are visible only to administrators. Default state of Product is notPublished. - notPublished or published |
|  displayName | string | Yes | Product name. |

