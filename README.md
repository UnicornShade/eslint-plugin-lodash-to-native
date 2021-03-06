# eslint-plugin-lodash-to-native

Replace lodash methods with ES6

## Installation

You'll first need to install [ESLint](http://eslint.org):

```
$ npm i eslint --save-dev
```

Next, install `eslint-plugin-lodash-to-native`:

```
$ npm install github:unicornshade/eslint-plugin-lodash-to-native --save-dev
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-lodash-to-native` globally.

## Usage

Add `lodash-to-native` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
    "plugins": [
        "lodash-to-native"
    ]
}
```


Then configure the rules you want to use under the rules section.

```json
{
    "rules": {
        "lodash-to-native/map": 2
    }
}
```

## Supported Rules

* map — checks `_.map` method and fixes it with native `Array.prototype.map` if can

## Tests

To run tests run command

```
$ npm run tests
```
