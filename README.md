## ONDC /vlookup UTILITY

1. Clone the repository, navigate to vlookup-ondc and install the dependencies.

```sh
cd vlookup-ondc
npm i
```

2. Import the vLookUp method in your project.

```js
const { vLookUp } = require("./index");

vLookUp({
  senderSubscriberId: "", //subscriber_id of sender
  privateKey: "", //private key of sender in base64 encoding

  //search parameters of the NP whose details need to be fetched from registry
  domain: "nic2004:52110",
  subscriberId: "buyerApp.com",
  country: "IND",
  type: "buyerApp", //buyerApp, sellerApp, gateway
  city: "std:080",
  env: "preprod", //preprod,prod
});
```

3. The output will consist of the registry details of the NP.
