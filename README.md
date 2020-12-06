# @creeation/prettier-config

![GitHub package.json version](https://img.shields.io/github/package-json/v/creeation/prettier-config?style=flat-square)
![npm (scoped)](https://img.shields.io/npm/v/@creeation/prettier-config?style=flat-square)
![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/creeation/prettier-config?style=flat-square)

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
