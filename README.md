# @creeation/prettier-config

[![npm (scoped)](https://img.shields.io/npm/v/@creeation/prettier-config?style=flat-square)](https://www.npmjs.com/package/@creeation/prettier-config)
[![GitHub package.json dependency version (dev dep on branch)](https://img.shields.io/github/package-json/dependency-version/creeation/prettier-config/dev/prettier?style=flat-square)](https://www.npmjs.com/package/prettier/v/2.2.1)
[![NPM](https://img.shields.io/npm/l/@creeation/prettier-config?style=flat-square)](https://github.com/CREEATION/prettier-config/blob/main/LICENSE)

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

## Configuring Prettier

- [Options](https://prettier.io/docs/en/options.html)
- [Configuration File](https://prettier.io/docs/en/configuration.html)

## Package Development Scripts and Hooks

### [Git Hooks](https://git-scm.com/docs/githooks) (using [Husky](https://typicode.github.io/husky/) and [pretty-quick](https://github.com/azz/pretty-quick))

#### `pre-commit`

```console
$ npm run pretty-quick --staged
```

### npm [Scripts](https://docs.npmjs.com/cli/v7/using-npm/scripts)

#### `test`

Checks if package files are formatted correctly using Prettier

```console
$ npm test
```

#### `format`

Formats and saves all package files using Prettier

> _Note: bound to [`prepublishOnly`](https://docs.npmjs.com/cli/v7/using-npm/scripts#life-cycle-scripts)_

```console
$ npm run format
```

### npm [Life Cycle Scripts](https://docs.npmjs.com/cli/v7/using-npm/scripts#life-cycle-operation-order)

#### [`postinstall`](https://docs.npmjs.com/cli/v7/using-npm/scripts#npm-install)

```console
$ npx husky install
```

#### [`prepublishOnly`](https://docs.npmjs.com/cli/v7/using-npm/scripts#npm-publish)

```console
$ npm test && npx pinst --disable
```

#### [`postpublish`](https://docs.npmjs.com/cli/v7/using-npm/scripts#npm-publish)

```console
$ npx pinst --enable
```
