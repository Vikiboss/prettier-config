# @vikiboss/prettier-config

> Personal [Prettier](https://prettier.io/) config

## Features

```js
module.exports = {
  semi: false,
  singleQuote: true,
  arrowParens: 'avoid',
  htmlWhitespaceSensitivity: 'strict',
  editorconfig: true,
}
```

For full defaults config fields, see [`defaults.json`](defaults.json).

## Usage

### Install

```bash
# npm
npm i -D @vikiboss/prettier-config

# yarn
yarn add -D @vikiboss/prettier-config

# pnpm
pnpm i -D @vikiboss/prettier-config
```

### Edit your config

you can add `prettier` field to your `package.json`:

```json
{
  // ...
  "prettier": "@vikiboss/prettier-config"
}
```

or add a `.prettierrc` file that contains following strings:

```json
"@vikiboss/prettier-config"
```

or you may want to **override** some rules based on it:

```js
// .prettierrc.js
module.exports = {
  ...require('@vikiboss/prettier-config'),
  semi: true,
  singleQuote: false,
  arrowParens: 'always',
}
```

## @vikiboss/prettier-config/fun

You will like it, maybe. 🤣

Just require config from `fun` and try it multiple times to see what will happen.

```js
// .prettierrc.js
module.exports = require('@vikiboss/prettier-config/fun')
```

## License

[MIT](LICENSE) License © 2022-PRESENT Viki
