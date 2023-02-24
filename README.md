<div align="center">

<br>

<h1>landing-grid</h1>

[![npm](https://img.shields.io/npm/v/landing-grid.svg?colorB=brightgreen)](https://www.npmjs.com/package/landing-grid)
[![GitHub package version](https://img.shields.io/github/package-json/v/ux-ui-pro/landing-grid.svg)](https://github.com/ux-ui-pro/landing-grid)
[![NPM Downloads](https://img.shields.io/npm/dm/landing-grid.svg?style=flat)](https://www.npmjs.org/package/landing-grid)

<sup>370 bytes gzipped</sup>
<h3><a href="https://ux-ui-pro.github.io/landing-grid/dist/">Demo</a></h3>

<sub>
This grid is designed to create a landing pages and has corresponding functional limitations.
</sub>


</div>
<br>

### Import
<sub>Import file if your bundler supports SCSS.</sub>
```SCSS
@import "node_modules/landing-grid/src/landing-grid.scss";
```
```SCSS
@import url("/node_modules/landing-grid/src/landing-grid.scss") screen and (min-width: 992px);
```
<sub>Or link to the file by the `<link>` element:</sub>
```HTML
<link rel="stylesheet" href="path-to-the-file/landing-grid.min.css">
```
<br>

### Usage
```CSS
:root {
    --wrapper: min(1600px, 92vw);
    --gutter: 3vw;
}
```
```HTML
<div class="wrapper">
	<div class="column" style="--column: 2; --offset: 2;">column 2 offset 2</div>
	<div class="column" style="--column: 5;">column 5</div>
	<div class="column column--infinite" style="--column: 3;">column 3 infinite</div>
</div>
```
<br>

### Settings

| Class&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
| --- | --- |
| `.wrapper` | ... |
| `.column` | ... |
| `.column--infinite` | Stretches the first or last column to the edge of the screen. |
<br>

| Variable&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
| --- | --- |
| `--wrapper` | Sets the width of the wrapper and the size of the margins from the wrapper on the left and right. For example: `80vw` or `calc(100vw - 100px)` or `min(1600px, 92vw)`. |
| `--gutter` | Sets the size of the margins between the columns. |
| `--column` | Used to set the width of one column. Allowed to use positive decimals. Example: `--column: 3.5`. |
| `--offset` | Move columns to the right using `--offset` variables. These variables increase the left margin of a column. For example, `--column: 8; --offset: 4;`. |
<br>

### License
<sub>landing-grid is released under MIT license.</sub>