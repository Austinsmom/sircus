# [sircus](http://sircus.blivesta.com)

[![npm version](https://img.shields.io/npm/v/sircus.svg?style=flat)](https://www.npmjs.com/package/sircus)
[![Build Status](https://img.shields.io/travis/sircus/sircus/master.svg?style=flat)](https://travis-ci.org/sircus/sircus)


## Install

npm:
```
$ npm install sircus
```

bower:
```
$ bower install sircus
```

## Usage

> Use [cssnext](http://cssnext.io/)

Create `input.css`
```css
@import "sircus";
```

Build
```
$ npm install cssnext
$ cssnext input.css output.css
```

> if use sass([node-sass](https://github.com/sass/node-sass))

Create `input.scss`

```css
@import "node_modules/sircus/sass";
```

```
$ npm install node-sass
$ node-sass input.scss output.css
```

## Modules
###  1: Global Module

- [sircus-global-property](https://github.com/sircus/global-property)

**variables**

`--g-variablesName-propertyName`


| Prefix   | e.g.               |
|:---------|:-------------------|
| `--g-*`  | `--g-primary-dark` |


### 2: Elements Module

- [sircus-elements-body](https://github.com/sircus/elements-body)
- [sircus-elements-heading](https://github.com/sircus/elements-heading)
- [sircus-elements-image](https://github.com/sircus/elements-image)
- [sircus-elements-link](https://github.com/sircus/elements-link)
- [sircus-elements-list](https://github.com/sircus/elements-list)
- [sircus-elements-paragraph](https://github.com/sircus/elements-paragraph)
- [sircus-elements-space](https://github.com/sircus/elements-space)

**variables**

`--elementsName-propertyName`


### 3: Components Module

- [sircus-components-alert](https://github.com/sircus/components-alert)
- [sircus-components-button](https://github.com/sircus/components-button)
- [sircus-components-button-fill](https://github.com/sircus/components-button-fill)
- [sircus-components-button-size](https://github.com/sircus/components-button-size)
- [sircus-components-button-reset](https://github.com/sircus/components-button-reset)
- [sircus-components-container](https://github.com/sircus/components-container)
- [sircus-components-flex](https://github.com/sircus/components-flex)
- [sircus-components-fullembed](https://github.com/sircus/components-fullembed)
- [sircus-components-form](https://github.com/sircus/components-form)
- [sircus-components-form-size](https://github.com/sircus/components-form-size)
- [sircus-components-grid](https://github.com/sircus/components-grid)
- [sircus-components-list](https://github.com/sircus/components-list)
- [sircus-components-table](https://github.com/sircus/components-table)

**variables**

`--ConmponentName-propertyName`

### Classies

Inspired by [SUIT CSS naming conventions](https://github.com/suitcss/suit/blob/master/doc/naming-conventions.md)

> [namespace-]ComponentsName[--modifierName|-descendentName]

```html
<div class="FullEmbed FullEmbed--16by9">
  <div class="FullEmbed-item"></div>
</div>
```

> ComponentName

- ** The component's name must be written in pascal case. **

```css
.FullEmbed { }
.Container { }
```
- if using namespace

> namespace-ComponentName

```css
.namespace-FullEmbed { }
```

> ComponentsName--modifierName

```css
.FullEmbed--16by9 { }
```

> ComponentsName-descendentName

```css
.FullEmbed-item { }
```

> ComponentsName.is-stateOfModule

```css
.Button { }
.Button.is-active { }
```

```html
<a class="Button is-active"> </a>
```
#### State classies

> .is-[focus||active||disabled]

* active
* focus
* disable

| Prefix   | e.g.               |
|:---------|:-------------------|
| `is-*`   | `is-active`        |



### 4: Tools Module

- [sircus-tools-align](https://github.com/sircus/tools-align)
- [sircus-tools-align-responsive](https://github.com/sircus/tools-align-responsive)
- [sircus-tools-clear](https://github.com/sircus/tools-clear)
- [sircus-tools-display](https://github.com/sircus/tools-display)
- [sircus-tools-display-responsive](https://github.com/sircus/tools-display-responsive)
- [sircus-tools-gutter](https://github.com/sircus/tools-gutter)
- [sircus-tools-gutter-responsive](https://github.com/sircus/tools-gutter-responsive)
- [sircus-tools-layout](https://github.com/sircus/tools-layout)
- [sircus-tools-layout-responsive](https://github.com/sircus/tools-layout-responsive)
- [sircus-tools-overflow](https://github.com/sircus/tools-overflow)
- [sircus-tools-overflow-responsive](https://github.com/sircus/tools-overflow-responsive)
- [sircus-tools-space](https://github.com/sircus/tools-space)
- [sircus-tools-space-responsive](https://github.com/sircus/tools-space-responsive)
- [sircus-tools-typography](https://github.com/sircus/tools-typography)
- [sircus-tools-width](https://github.com/sircus/tools-width)
- [sircus-tools-width-responsive](https://github.com/sircus/tools-width-responsive)

**variables**

> --toolName-propertyName

| Prefix   | e.g.            |
|:---------|:----------------|
| `none`   | `--gutter-size` |


#### Classies

`t-[sm-||md-||lg-]toolName`

```css
.t-clear { }
.t-sm-block { }
.t-xs-width2of4 { }
```

```html
<div class="t-clear">
  <div class="t-left t-xs-hidden"></div>
  <p class="t-uppercase"></p>
</div>
```


## Abbreviations

Default viewports

| variables            | min-width         |
|:---------------------|:------------------|
| --g-viewport-sm    | 40em = 640px      |
| --g-viewport-md    | 64em = 1024px     |
| --g-viewport-lg    | 75em = 1200px     |


Size level Suffix

| abbr (Suffix) | Base            | Level |
|:--------------|:----------------|:------|
| *-gt          | Gargantuan      | +4    |
| *-hg          | Huge            | +3    |
| *-xl          | Extra Large     | +2    |
| *-lg          | Large           | +1    |
| *-bs(md)      | Base (Medium)   | 0     |
| *-sm          | Small           | -1    |
| *-xs          | Extra Small     | -2    |
| *-tn          | Tiny            | -3    |
| *-mn          | Minimal         | -4    |
| *-nn or 0     | None            | 　    |


## Development
```
$ git clone https://github.com/sircus/sircus.git
$ cd sircus
$ git checkout -b patch-1
$ npm run start
```

## Resources

**[cssnext](http://cssnext.io/)**

> Use tomorrow's CSS syntax, today


## Contributing

We Need Your Help!


## License
Released under the [MIT](https://github.com/sircus/license/blob/master/LICENSE) license.
