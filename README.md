# @creeation/prettier-config

[![GitHub package.json version](https://img.shields.io/github/package-json/v/creeation/prettier-config?style=flat-square)](https://github.com/CREEATION/prettier-config)
[![npm (scoped)](https://img.shields.io/npm/v/@creeation/prettier-config?style=flat-square)](https://www.npmjs.com/package/@creeation/prettier-config)
[![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/npm/@creeation/prettier-config?style=flat-square)](https://www.npmjs.com/package/@creeation/prettier-config?activeTab=dependencies)

Repository holding my personal Prettier configuration.

## Installation

```console
$ npm i -D @creeation/prettier-config
```

Then, in your `package.json`, set `prettier` to `@creeation/prettier-config`:

```json
{
  "prettier": "@creeation/prettier-config"
}
```

## Package Development Scripts and Callbacks

### `test`

Checks if package files are formatted correctly using Prettier

> Note: bound to [`prepare`](https://docs.npmjs.com/cli/v6/using-npm/scripts#life-cycle-scripts)

```console
$ npm run test
```

### `format`

Formats and saves package files using Prettier

> Note: bound to [`prepublishOnly`](https://docs.npmjs.com/cli/v6/using-npm/scripts#life-cycle-scripts)

```console
$ npm run format
```

---

**Keywords**: `creeation`, `prettier`, `prettierconfig`, `prettier-config`
