# SCSS Function Em

Пакет для интеграции функции преобразования `px` в `em`.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-em?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-em?style=for-the-badge)

Документация: [EN](README.md) | [RU](README.RU.md)

___

## Установка

Вы можете установить пакет автоматически с помощью NPM:

```
npm i @bu0nq/scss-function-em
```

## Использование

Чтобы использовать этот пакет, импортируйте его в свой проект:

```scss
@use "@bu0nq/scss-function-em" as *;

.demo {
    font-size: em(16px);
}
```

## Изменение пространства имен

Вы можете изменить пространство имен во время импорта функции и использовать функцию с другим пространством имен:

```scss
@use "@bu0nq/scss-function-em" as function;

.demo {
    font-size: function.em(16px);
}
```

## Изменение переменных

Вы можете переопределить значения по умолчанию для указанных переменных при импорте функции:

```scss
@use "@bu0nq/scss-function-em" as * with (
    $baseline: 16,
);
```
