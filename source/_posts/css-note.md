---
title: css-note
date: 2021-10-25 10:09:08
tags: css
toc: true
---

# CSS selectors

```css
h1,
h2,
h3 {
  ...;
} /* html tag selector */

#id {
  ...;
} /* id selector */

.class {
  ...;
} /* class selector */

.class img {
  ...;
} /* descendant combinator */

.class:hover {
  ...;
} /* user action pseudo class */

.class:nth-of-type(odd) {
  ...;
} /* location pseudo class
nth-of-type: number or odd/even
first-of-type/last-of-type
nth-child
first-child/last-child
*/

#leftmenu > ul > li > a {
  ...;
} /* child combinator */

.sidebar + h2 {
  ...;
} /* adjacent sibling combinator */

.sidebar ~ h2 {
  ...;
} /* general sibling combinator */
```

# CSS property reference

## text style

```css
color: white; /* default black */
font-size: 18px; /* default 16px */
font-weight: bold; /* default normal */
font-style: italic; /* default normal */

/* whitespace between lines of test */
line-height: 1.5; /* default 1, relative to font-size */
/* space between characters */
letter-spacing: 2px; /* default 0 */

/* visit cssfontstack.com to find more web-safe fonts. */
font-family: Verdana, Arial, sans-serif, cursive, fantasy; /* web-safe fonts, default Arial */
/* serif: Georgia, Times New Roman
sans-serif: Arial, Verdana, Comic Sans, Trebuchet
monospace: Courier New */

text-align: center; /* justify, default left */
text-transform: capitalize; /* uppercase, default none */
```

## container style

The Box Model: element < padding < border < margin

Use chrome dev tools to inspect the box model.

```css
width: 100%;
/* relative to parent width, default auto
width: 1em; relative to parent font-size
width: 1rem; relative to html font-size */

background-color: #23cea6; /* RGB, default transparent */
border: 10px solid #a693c2;
border-color: #a693c2;
/* border inside, width, style, color(default text color)
style: solid, dashed, dotted, ridge, double, groove, inset, outset
border-left: xxx; left only */
outline: 10px solid red; /* border outside */

padding: 10px 20px 30px 40px;
/* space between container and content
top right bottom left
top/bottom left/right
top/right/bottom/left */
padding-left: 10px;

margin: 10px 20px 30px 40px;
/* space between container and next element
margin collapse, max(margin-bottom, margin-top) applied */
margin-bottom: 10px;
```
