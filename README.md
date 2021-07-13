# singleton-event-emitter

A singleton instance of node EventEmitter. If it is required in multiple node packages, it will return the same instance of EvenetEmitter.
Can be used to emit global debug events.

## Installation

```bash
npm install singleton-event-emitter
```

## Usage

```js
// emitter.js
const singletonEvenetEmitter = require('singleton-evenet-emitter');
singletonEvenetEmitter.emit('someEvent')

// listener.js
const singletonEvenetEmitter = require('singleton-evenet-emitter');
singletonEvenetEmitter.on('someEvent', () => {
	console.log("someEvent");
})
```

