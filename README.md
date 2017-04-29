# rollup-regenerator-runtime

Use this to add regenerator to any library that's compiled using rollup.

## Installation

N.B. because rollup will compile everything into one bundle, you can install everything as a dev-dependency

```
npm install --save-dev rollup-regenerator-runtime babel-plugin-transform-runtime babel-plugin-transform-regenerator
```

## Usage

```
{
  "plugins": [
    "transform-regenerator",
    ["transform-runtime", {
      "helpers": false,
      "polyfill": false,
      "regenerator": true,
      "moduleName": "rollup-regenerator-runtime"
    }]
  ]
}
```
