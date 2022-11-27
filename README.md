---

A library that allows you to use the new extension to store data. Working with it is very simple. You can get data, change, create, etc.

---

- [Getting Started](#getting-started)
- [etc Authentications](#etc-authentications)
  - [Experimenting](#experimenting)

## Getting Started

To apply etc to your project:
```js
// In a node.js environment
const ETC = require('etc')('file.etc') // ('file.etc') open file.etc
```

Sample code for using etc, in node.js;
```js
let etc = "und": {
	"id": "und";
	"book": "und"
};

let etc = "etc": {
	"id": "39";
	"book": "js"
};

let etcup = "etcupd": {
	"id": "40";
	"book": "shiooo"
};

ETC
  .pipeAsyncStorage(etc) // OK
  .updAsyncStorage(etc, etcupd) // OK
  .delAsyncStorage(und) // und is not defined!

let up = ETC.getAsyncStorage("etcupd")

console.log(ETC.getAsyncStorage("etcupd")) // "etcupd": { "id": "40"; "book": "shiooo" };
console.log(up.id) // "40"

if (ETC.getAsyncStorage("etc") === Error) {
	console.log('Is deleted!')
} else {
	console.log('Error... Obj exists')
}
```

## etc Authentications
OK
### Experimenting
You can install the etc extension using:
```
npm install etc@latest or npm install etc@0.0.7
```
