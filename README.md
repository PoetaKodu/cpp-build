# cpp-build
An easy to use C++ build system.

## Usage:

To compile single `main.cpp` file, create `build.js` file:

```js
const cb = require("cpp-build");

let main_cpp = new cb.File("main.cpp", [ "-std=c++11" ]);

cb.export(module, main_cpp);
```

Run `cpp-build` as following:

```plaintext
mkdir build
cd build
node cpp-build -g -b ../build.js
```

