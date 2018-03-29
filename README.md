# 🌈✋ Common Colors css

A "human" CSS color scheme with *unambiguous* color names, at your fingertips.
Demo & color chart:  <https://juytter.github.io/common-colors-css/>

---

## Benefit

Provide a simple 'human' interface for naming, choosing, using, and sharing colors in a project :

- no need for color codes
- no necessarily need a color chart to choose hues.

[Introducing](https://github.com/juytter/common-colors-css/introducing.html) Common Colors css

## Download

- [Releases](https://github.com/juytter/common-colors-css/releases)
- [Last version (zip)](dist/common-colors-css-lastest.zip)

## Usage

#### CSS vars

The obvious way to use *common colors* is using [css variables](http://devdocs.io/css/--*). (css var is currently *experimental*, but can be used with css preprocessors, such as [postcss](https://github.com/postcss/postcss) ).

import [common-colors--vars.css](css/common-colors--vars.css)

```css
@import 'common-colors--vars.css';
.warning { color : var(--red); }
.warning-alt { color : var(--red-pale); }
```

#### Common-colors css libs

Actually the best reliable way to integrate Common-colors Css and color names into a project.

Link [common-colors.css](css/common-colors.css) or [minified](css/min/common-colors.min.css) (4 Ko) lib to color *text* and *background* with class names.

##### Apply colors

```html
<p class="red"></p>
<p class="red-pale"</p>
```

##### Apply background colors  (add a prefix `bg-` )

```html
/* white on red background */
<div class="bg-red white"></div>
```

##### Common-colors css lib - Extra

Link [common-colors-extra.css](css/common-colors-extra.css) or [minified](css/min/common-colors-extra.min.css) to color *borders* and *pseudo* (hover/focus) on elements with class names

```html
/* red border */
<p class="border bd-red"></p>
/* yellow color, yellow-black on hover */
<a class="yellow hv_yellow-black"></a>
```

##### Alt. specific CSS files

See. [/css](/css)


## Build & contribute   

- [Contributing](CONTRIBUTING.md)
- Sources [/src](/src)
- Tools and dependencies [package.json](package.json)
- Build script  [gulpfile.js](gulpfile.js),  command line :  `gulp build`
