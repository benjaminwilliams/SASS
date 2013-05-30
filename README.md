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


_helpers.scss
---------------------
Adds padding and margin helpers in each direction between 10px and 50px (in 10px incriments)

#### Examples

	.margin-top-10 
	.margin-right-30
	.padding-bottom-10
	.padding-left-20