# SCSS Function Em

A package for integrating the `px` to `em` conversion function.

Documentation: [EN](README.md) | [RU](README.RU.md)

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-em?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-em?style=for-the-badge)
___

## Installation

You can install the package automatically using NPM:

```
npm i @bu0nq/scss-function-em
```

## Usage

To use the package, import it into your project:

```scss
@use "@bu0nq/scss-function-em" as *;

.demo {
    font-size: em(16px);
}
```

## Changing the namespace

You can change the namespace during function import and use the function with a different namespace:

```scss
@use "@bu0nq/scss-function-em" as function;

.demo {
    font-size: function.em(16px);
}
```

## Changing the variables

You can redefine the default values for the specified variables when importing the function:

```scss
@use "@bu0nq/scss-function-em" as * with (
    $baseline: 16,
);
```
