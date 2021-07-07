# Readme for the `babel-preset-core` preset.
#

This preset is a lightweight `.babelrc` preset that enables most features of Babel core, plus some extras.

We will not be introducing any plugins here, however the following plugins are available:

- [object-curly-new-line](https://github.com/zertosh/babel-preset-object-curly-new-line)
- [function-bind](https://github.com/lodash/lodash)
- [class-properties](https://github.com/jonschlinkert/object-curly-constructor)
- [create-react-class](https://github.com/SvenZW/create-react-class)
- [lodash-es](https://github.com/SvenZW/lodash-es)
- [babel-plugin-macros](https://github.com/vadimdemedes/babel-plugin-macros)
- [babel-plugin-minify](https://github.com/MaxDimPy/babel-plugin-minify)

## Installation

```sh
# Node.js
npm install --save-dev babel-preset-core

# Browser
yarn add babel-preset-core
```

## Usage

**Note**:

* This preset will **not** work without the `.babelrc` file that was initially installed.
* This preset **will not** take effect if `.babelrc` file doesn't include the preset itself (`plugins: [babel-preset-core]`).
* If you choose to specify a value for `env: production`, please also add a value for `presets: [babel-preset-env]` or include it directly.

## Why this preset?

- [es2015](https://babeljs.io/docs/en/babel-preset-es2015), `stage-0`, `stage-1`, `stage-2` and `stage-3` are the main targets of this preset
- it has [all ES2015+ features](https://github.com/SvenZW/babel-preset-es2015) and [full support for the latest stages of the specification](https://github.com/SvenZW/babel-preset-es2015#features)
- it has [full support for Object rest/spread](https://github.com/SvenZW/babel-preset-es2015#options)

## API

> [babel-preset-es2015](https://github.com/babel/babel-preset-es2015)

```json
{
  "presets": [
    "@babel/preset-es2015"
  ],
  "plugins": [
    "react-display-name"
  ]
}
```

- `presets` - Array of the presets
- `plugins` - Array of the plugins

## License

MIT © [Sven Zanker](https://github.com/SvenZW)
