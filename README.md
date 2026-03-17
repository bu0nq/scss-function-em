# SCSS Function Em

Package for integrating `SCSS Function Em` in a web environment.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-em?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-em?style=for-the-badge)
___

## Installation

This package can be deployed automatically using NPM:

```
npm i @bu0nq/scss-function-em
```

## Usage

Import in your project depending on your setup:

```scss
@use "@bu0nq/scss-function-em" as *;

.demo {
    font-size: em(16px);
}
```

## Namespace

You can change the namespace during import and use the em function with a different namespace:

```scss
@use "@bu0nq/scss-function-em" as to;

.demo {
    font-size: to.em(16px);
}
```

## Changing baseline

By default, `function-em` uses a base size of 16 pixels, but you can change this value using the `$baseline` command and using the baseline parameter to adjust the size of the main font.

```scss
@use "@bu0nq/scss-function-em" as * with (
  $baseline: 10
);

.demo {
    font-size: em(16px);
}
```

Execution result:

```css
.demo {
    font-size: 1.6em;
}
```
