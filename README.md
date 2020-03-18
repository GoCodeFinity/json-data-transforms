# Data Conversion Utilities

In the process of doing some conversion of JSON data using, it seemed worthwile to build a basic 'utils library' of sorts.

As usual, do `npm i` to get started after cloning. There are some VS Code extensions and settings included.ß

No JSON data is actually included, but you can keep it there in JSON and read the info in. For example, if you have some 'json/catalog.json':

```js
// Use 'promisified' version of 'fs' from 'newer' Node.
import { promises as fs } from "fs";

// Using 'async' IIFE
(async function() {
  const catalog = JSON.parse(await fs.readFile("./json/catalog.json"));

  /**
   * TODO: Import and invoke some fxns. from './lib.js.'
   * 'writeFile' JSON back.
   */
})();
```

---

Alternatively, just copy/paste whatever is needed out of './lib.js.'
