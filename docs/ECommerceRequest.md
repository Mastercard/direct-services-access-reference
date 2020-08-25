# ECommerceRequest

## Properties <a name="properties"></a>
All properties for the request object are listed in the [Direct Service Request](docs/models/DirectServiceRequest.md) page.

The sample below provides the specific fields required by the e-commerce use case.

## Sample JSON

```json
{
  "serviceType": "ORIGINAL",
  "clientTransactionId": "12345",
	"customer": {
	    "id": "567899"
	},
	"card": {
		"accountNumber": "5400000000000000",
		"expiry": "2020-12",
		"validationCode": "567",
		"sequenceNumber": 891      
	},
	"transaction": {
		"transactionType": "00",
		"fromAccountType":"00",
		"toAccountType": "00"
	},
	"terminal": {
		"panEntryMode": "CONTACTLESS_MAGNETIC_STRIPE"
	},
	"cardAcceptor": {
		"merchantType": "5499"
	},
	"security": {
		"chipData": "AQJeCgULCwcOA18KBQsEBwNfCgULBAc=",
		"universalCardholderAuthenticationField": "aduX3UYzkZWYd_JQ1FbXcaBa",
		"pinBlock": "MTIzNDU2Nzg=",
		"pinBlockFormat": "ISO_FORMAT_0",
		"pinKeyIndex" :	"1234",
 		"digitalPayment":{
			"cryptogram": "AQJeCgULCwcOA18KBQsEBwNfCgULBAc=",
			"merchantId": "d3d3Lm1hY3lzLmNvbQ=="
		}
	},
	"authentication": {
		"securityProtocol": "1",
		"cardholderAuthentication":"2",
		"ucafCollectionIndicator": "3"
	}
}
```