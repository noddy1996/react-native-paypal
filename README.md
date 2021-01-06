
# react-native-paypal
A wrapper for the paypal sdk for both android and ios.

## Getting started

`$ yarn add react-native-paypal-module`


## Usage
```javascript
import RNPaypal from 'react-native-paypal-module';

RNPaypal.paymentRequest({
    clientId: '<YOUR CLIENT ID>',
    environment: RNPaypal.ENVIRONMENT.NO_NETWORK,
    intent: RNPaypal.INTENT.SALE,
    price: 60,
    currency: 'USD',
    description: `Android testing`,
    acceptCreditCards: true
}).then(response => {
    console.log(response)
}).catch(err => {
    console.log(err.message)
})
```
  