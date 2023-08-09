# @vmoe/prettier-config

> Viki's shareable [Prettier](https://prettier.io) config.

## Features

```js
module.exports = {
  htmlWhitespaceSensitivity: 'strict',
  vueIndentScriptAndStyle: true,
  printWidth: 100,
  semi: false,
  singleQuote: true,
}
```

For full prettier default config, head to [`defaults.json`](defaults.json).

## Usage

### Install

```bash
# npm
npm i -D @vmoe/prettier-config

# yarn
yarn add -D @vmoe/prettier-config

# pnpm
pnpm add -D @vmoe/prettier-config
```

### Edit your config

add `prettier` field to your `package.json`:

```jsonc
{
  "name": "awesome-project",
  // ...
  "prettier": "@vmoe/prettier-config"
  // ...
}
```

or add a `.prettierrc` file that contains following string:

```json
"@vmoe/prettier-config"
```

or you may want to **override** some rules based on it:

```js
// .prettierrc.js
module.exports = {
  ...require('@vmoe/prettier-config'),
  semi: true,
  singleQuote: false,
}
```

## @vmoe/prettier-config/fun

You will like it, maybe. 🤣

Just require config from the `fun` path and try it multiple times to see what will happen.

```js
// .prettierrc.js
module.exports = require('@vmoe/prettier-config/fun')
```

## License

[MIT](LICENSE) License © 2022-PRESENT Viki
