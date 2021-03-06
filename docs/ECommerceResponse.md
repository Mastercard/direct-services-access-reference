# ECommerceResponse

## Properties <a name="properties"></a>
All properties for the request object are listed in the [Direct Service Response](docs/models/DirectServiceResponse.md) page.

The sample below provides the specific fields required by the e-commerce use case.

## Sample JSON

```json
{
  "response": {
    "responseCode": "12",
    "clientTransactionId": "03vLwCxtn3/pZCliH5mXY1Bozs5HspdIdn20H/GTRrU=",
    "mastercardReferenceId": "00NPAN",
    "card": {
      "accountNumber": "5400000000000000",
      "expiry": "2023-01"
    },
    "security": {
      "pinBlock": "AQJeCgULCwc=",
      "digitalPayment": {
        "merchantId": "d3d3Lm1hY3lzLmNvbQ=="
      }
    },
    "authentication": {
      "securityProtocol": 9,
      "cardholderAuthentication": 0,
      "ucafCollectionIndicator": 0
    }
  },
  "request": {
    "serviceType": "ORIGINAL",
    "clientTransactionId": "03vLwCxtn3/pZCliH5mXY1Bozs5HspdIdn20H/GTRrU=",
    "customer": {
      "id": "567899"
    },
    "card": {
      "accountNumber": "5400000000000000",
      "expiry": "2023-12",
      "validationCode": "567",
      "sequenceNumber": "891"
    },
    "transaction": {
      "transactionType": "00",
      "fromAccountType": "20",
      "toAccountType": "20",
      "amount": 50000
    },
    "terminal": {
      "panEntryMode": "CONTACTLESS_MAGNETIC_STRIPE"
    },
    "cardAcceptor": {
      "merchantType": "5499"
    },
    "security": {
      "chipData": "NUYyQTAyMDk3ODgyMDI1QzAwOTUwNUFCMjZGQkNEQjE5QTAzMDMwNjE5OUMwMTAwOUYwMjA2MDAwMDAwMDEwMDAwOUYxMDEyMDAxMkUxMjM0QkM3QkJDQzk2MUYwMDAwMDAwMDAwMDAwMEZGOUYxQTAyMDg0MDlGMjcwMTgwOUYzNjAyMDBBMjlGMzcwNDAwMDAwMDU2OUYyNjA4N0FDMjEzMEM3OEQyQTQ3Mw==",
      "universalCardholderAuthenticationField": "aduX3UYzkZWYd_JQ1FbXcaBa",
      "pinBlock": "AQJeCgULCwc=",
      "pinBlockFormat": "ISO_FORMAT_0",
      "pinKeyIndex": 98,
      "digitalPayment": {
        "merchantId": "d3d3Lm1hY3lzLmNvbQ=="
      }
    },
    "authentication": {
      "securityProtocol": 9,
      "cardholderAuthentication": 0,
      "ucafCollectionIndicator": 0
    }
  }
}
```
