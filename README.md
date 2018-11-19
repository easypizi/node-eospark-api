# Node.js EosPark API

Node.js package to interact with official [EosPark API](https://eospark.com/openapi)

## Documentation

**[API reference](https://github.com/easypizi/node-eospark-api/blob/master/README.md)**

The API reference was generated by JSDoc.
If you use Typescript, you can use the more detailed reference found in the [type declaration file](https://github.com/danakt/node-eospark-api/blob/master/index.d.ts)

This library and codestyle is based on node-etherscan-api by Danakt Frost;

## Install

```bash
$ npm install node-eospark-api
```

## Usage

```js
const EosparkConnect = require("node-etherscan-api");

// Replace the value below with the your Etherscan token
const TOKEN_API = "YourApiKeyToken";

// Creating the EosPark instance
const eospark = new EosparkConnect(TOKEN_API);

// Creating a request for account balance in Ether (default returns in Wei)

eospark
  .getAccountInfo("eosknightsio")
  .then(result => {
    // Working with the account data here
    console.log(balance);
  })
  .catch(err => {
    // Handle error here
    console.error(err);
  });
```

## License

**The MIT License (MIT)**

Copyright © 2018 Evan Tolstoff
