SASS Mixins
====================

_arrows.scss
---------------------
Allows you to place a css arrow easily onto an element.

#### Basic syntax

`@include arrow($size, $dir, $color, $border-width, $border-color);`

	$size - Size of arrow
	$pos - Position (top, bottom, left, right)
	$color - Arrow colour 
	$border-width - border width (use 0 for no border)
	$border-color - border colour (use 0 for no border)


#### Examples 

@include arrow(15px, left, #999, 2, #444);

@include arrow(20px, top, #999, 0, 0);


_gradient.scss
---------------------
Add a background gradient to any element. Full cross browser compatibility with solid colour fallback.
original css compiled from [colorzilla.com/gradient-editor/](http://www.colorzilla.com/gradient-editor/)

#### Basic syntax

`@include gradient($dir, $R1, $G1, $B1, $A1, $R1, $G1, $B1, $A1);`

	$dir - Direction of gradient (up, down)
	$R1, $G1, $B1, $A1 - First RGBA colour eg "225,255,255,1" for white
	$R1, $G1, $B1, $A1 - Second RGBA colour eg "225,255,255,0.5" for white, 50% opacity

#### Examples 

A nice horrible white to black gradient: 
	@include gradient(down, 255, 255, 255, 1, 0, 0, 0, 1);

A subtle blue background: 
	@include gradient(down, 0, 122, 229, 1, 0, 70, 234, 1);

The same blue background reversed with a little transparency: 
	@include gradient(up, 0, 122, 229, 0.8, 0, 70, 234, 0.8);




_helpers.scss
---------------------
Adds padding and margin helpers in each direction between 10px and 50px (in 10px incriments)

#### Examples

	.margin-top-10 
	.margin-right-30
	.padding-bottom-10
	.padding-left-20