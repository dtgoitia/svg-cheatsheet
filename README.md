# SVG cheatsheet

## Cheatsheet structure
<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=3 orderedList=false} -->
<!-- code_chunk_output -->

* [Cheatsheet structure](#cheatsheet-structure)
* [Basic shapes](#basic-shapes)
	* [Paths](#paths)
	* [Rectangle](#rectangle)
	* [Circle](#circle)
	* [Ellipse](#ellipse)
	* [Line](#line-1)
	* [Polyline](#polyline)
	* [Polygon](#polygon)
* [Strokes](#strokes)
* [Fills](#fills)
* [External resources](#external-resources)

<!-- /code_chunk_output -->

> **CAVEAT**
This sheet doesn't aim to cover all SVG features.

## Basic shapes

### Paths

```html
<path
  d="M 20 230 Q 40 205, 50 230 T 90230 Z"
  fill="transparent"
  stroke="black"
/>
```

For all commands:  uppercase = **absolute** coordinates; lowercase = **relative** coordinates.

#### Line commands

There are 5 line commands for `<path>` node:
  * [Move](#move)
  * [Line](#line)
  * [Horizontal line](#horizontal-line)
  * [Vertical line](#vertical-line)
  * [Close Path](#close-path)

##### Move

```html
M  x  y   <!-- absolute coordinates -->
m dx dy   <!-- relative coordinates -->
```

##### Line

```html
L  x  y   <!-- absolute coordinates -->
l dx dy   <!-- relative coordinates -->
```

##### Horizontal line

```html
H  x  y   <!-- absolute coordinates -->
h dx dy   <!-- relative coordinates -->
```

##### Vertical line

```html
V  x  y   <!-- absolute coordinates -->
v dx dy   <!-- relative coordinates -->
```

##### Close Path

```html
z
```

#### Curve commands

##### Bezier Curves

TODO

Go to [MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#Bezier_Curves).

##### Arcs

```html
A rx ry x-axis-rotation large-arc-flag sweep-flag  x  y   <!-- absolute coordinates -->
a rx ry x-axis-rotation large-arc-flag sweep-flag dx dy   <!-- relative coordinates -->
```
Go to [MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#Arcs).

### Rectangle

TODO

### Circle

TODO

### Ellipse

TODO

### Line

TODO

### Polyline

TODO

### Polygon

TODO


## Strokes

```html
<polyline points="40 60 80 20 120 60" fill="none"
  stroke="black"
  stroke-width="20"
  stroke-dasharray="5,5"
  stroke-linecap="butt"
  stroke-linejoin="miter"
  stroke-opacity="0.8"
/>
```

## Fills

```html
<polyline points="40 60 80 20 120 60" stroke="none"
  fill="purple"
  fill-opacity="0.5"
  fill-rule="nonzero"
/>
```


## External resources

* [MDN | SVG tutorials](https://developer.mozilla.org/en-US/docs/tag/SVG:Tutorial)
* [MDN | Paths](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths)
* [MDN | Fills and Strokes](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Fills_and_Strokes)