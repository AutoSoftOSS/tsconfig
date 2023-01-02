<div align="center">
  <h1>@autosoft/tsconfig</h1>
  <a href="https://npmjs.com/package/autosoft/tsconfig">
    <img alt="npm" src="https://img.shields.io/npm/v/@autosoft/tsconfig.svg">
  </a>
  <a href="https://github.com/autosoftoss/tsconfig">
    <img alt="typescript" src="https://img.shields.io/github/languages/top/autosoftoss/tsconfig.svg">
  </a>
</div>

<br />

<blockquote align="center">A base for TypeScript projects.</blockquote>

_If I should maintain this repo, please ⭐️_
<a href="https://github.com/autosoftoss/tsconfig">
  <img align="right" alt="GitHub stars" src="https://img.shields.io/github/stars/autosoftoss/tsconfig?label=%E2%AD%90%EF%B8%8F&style=social">
</a>

_DM me on [Twitter](https://twitter.com/bconnorwhite) if you have questions or suggestions._
<a href="https://twitter.com/bconnorwhite">
  <img align="right" alt="Twitter Follow" src="https://img.shields.io/twitter/url?label=%40bconnorwhite&style=social&url=https%3A%2F%2Ftwitter.com%2Fbconnorwhite">
</a>

---

This package includes `typescript`, `ts-node`, and a base `tsconfig.json`, providing a quick way to start TypeScript projects.

## Installation

```sh
yarn add --dev @autosoft/tsconfig
```

```sh
npm install --save-dev @autosoft/tsconfig
```

```sh
pnpm add --save-dev @autosoft/tsconfig
```

## Usage

In your `tsconfig.json` file:

```json
{
  "extends": "@autosoft/tsconfig"
}
```

### TSC

To run TSC, run `yarn tsc` or `npm run tsc`.

### TS-Node

To run TS-Node, run `yarn ts-node` or `npm run ts-node`.

For ESM, run `yarn ts-node-esm` or `npm run ts-node-esm`.

## TSConfig

The config enable strict type checking, and includes SWC for ts-node:

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "compilerOptions": {
    "declaration": true,
    "esModuleInterop": true,
    "forceConsistentCasingInFileNames": true,
    "isolatedModules": true,
    "lib": [
      "ESNext",
      "DOM"
    ],
    "module": "ESNext",
    "moduleResolution": "Node",
    "noFallthroughCasesInSwitch": true,
    "noImplicitReturns": true,
    "noUncheckedIndexedAccess": true,
    "noUnusedLocals": true,
    "removeComments": false,
    "resolveJsonModule": true,
    "skipLibCheck": true,
    "strict": true,
    "target": "ES2019"
  },
  "ts-node": {
    "esm": true,
    "swc": true
  }
}
```

<br />

<h2 id="dependencies">Dependencies<a href="https://www.npmjs.com/package/autosoft/tsconfig?activeTab=dependencies"><img align="right" alt="dependencies" src="https://img.shields.io/librariesio/release/npm/@autosoft/tsconfig.svg"></a></h2>

- [@swc/core](https://www.npmjs.com/package/@swc/core): Super-fast alternative for babel
- [ts-node](https://www.npmjs.com/package/ts-node): TypeScript execution environment and REPL for node.js, with source map support
- [typescript](https://www.npmjs.com/package/typescript): TypeScript is a language for application scale JavaScript development

<h3 id="dev-dependencies">Dev Dependencies</h3>

- [jsonlint](https://www.npmjs.com/package/jsonlint): Validate JSON

<br />

<h2 id="license">License <a href="https://opensource.org/licenses/MIT"><img align="right" alt="license" src="https://img.shields.io/npm/l/@autosoft/tsconfig.svg"></a></h2>

[MIT](https://opensource.org/licenses/MIT)
