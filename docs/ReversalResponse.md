# ReversalResponse

## Properties <a name="properties"></a>
All properties for the request object are listed in the [Direct Service Response](docs/models/DirectServiceResponse.md) page.

The sample below provides the specific fields required by the reversal use case.

## Sample JSON

```json
{
  "response":{
    "responseCode":"12",
    "mastercardReferenceId":"0SBQAN",
    "card":{
      "accountNumber":"5400000000000000"}
    },
  "request":{
    "serviceType":"REVERSAL",
    "customer":{
      "id":"567899"
    },
    "card":{
      "accountNumber":"5400000000000000"
    },
    "original":{
      "responseCode":"00"
    }
  }
}
```