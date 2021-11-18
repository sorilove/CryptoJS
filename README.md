# crypto-jS.min

Javascript library of crypto-js without node crypto

## For Cocos Creator 3.x

CocosCreator 3.x can't use crypto an crypto-js, because creator is not base on nodejs.
So We could use this library crypto.min.js
to do crypto and API is the same as crypto-js

## Install

- Copy into CocosCreator
- Set crypto-js.min.js to "Import as plugin", - allow "Load in Web"、"Load in Native"、"Load in Editor", set the scope to independent, and simulate global variables as "CryptoJS"

## Usage

use without import and API the same as crypto-js, use case:

```javascript
//createEncryptor
CryptoJS.algo.AES.createEncryptor(key, { keySize: 4, iv: iv, model: CryptoJS.mode.CBC, padding: CryptoJS.pad.Pkcs7 });

```

## Tips
- Do not use crypto-js because node crypto
- Do not use crypto-ts because so mush bug
- Do not use any other crypto library such crypto-es、ase-js....
- You can set /* eslint-disable @typescript-eslint/no-unsafe-call */ for unsafe any call