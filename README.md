# crypto-jS.min

Javascript library of crypto-js without node crypto
노드 암호화가 없는 크립토-js의 자바스크립트 라이브러리

## For Cocos Creator 3.x

CocosCreator 3.x can't use crypto an crypto-js, because creator is not base on nodejs.
So We could use this library crypto.min.js
to do crypto and API is the same as crypto-js

CocosCreator 3.x는 크리에이터가 nodejs를 기반으로 하지 않기 때문에 크립토-js를 사용할 수 없습니다.
따라서 다음 라이브러리 crypto.min.js를 사용할 수 있습니다.

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
- Do not use crypto-js because node crypto (노드 암호화를 위해 암호-js를 사용하지 마십시오.)
- Do not use crypto-ts because so mush bug (너무 머쉬 버그 때문에 크립토-트를 사용하지 마십시오.)
- Do not use any other crypto library such crypto-es、ase-js.... (다른 암호화 라이브러리(예: crypto-es、ase-js....)를 사용하지 마세요.)
- You can set /* eslint-disable @typescript-eslint/no-unsafe-call */ for unsafe any call (안전하지 않은 모든 통화에 대해 /* eslint-disable @typescript-eslint/ no-unsafe-call */을 설정할 수 있습니다.)