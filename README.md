# conservative-tonejs

### Please go to official tonejs repository if you want to see the document of [Tone.js](https://github.com/Tonejs/Tone.js)
### This repository is a fork of Yotam Mann's Tone.js, which is mainly for personal usage.

### Thing that change

**Remove singleton of Transport, Destination, Master, Listener, Draw and context**

These singletons call getContext() when page is initializing. Therefore, the error from getContext will not be able to catch and such will caused whole webpage broken.

**Add polyfill for AudioParam.cancelAndHoldAtTime**

**Add polyfill for constant-source-node**

**Add polyfill for promise OfflineContext.startRendering**