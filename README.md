# Dynamic Response Media Sass Utilities

## Installation

+ Add utilities folder and _drm-sass-utilities.scss to project sass folder
+ Import _drm-sass-utilities.scss into main scss folder

## Documentation

### Media Query Breakpoints

	breakpoint deminsions can be customized in variables file

	+ trenta
	+ venti
	+ grande
	+ tall
	+ short
	+ espresso
	+ bean

			@include breakpoint(trenta) {
				// place rules here
			}

			@include breakpoint(venti) {
				// place rules here
			}

### Layout Utilities

+ %container

		@extend %container;

	+ Centers an element on the page
	+ for elements that take up the entire width of the wrapper
	+ includes built in breakpoints for responsiveness

+ %reset-box

		@extend %reset-box;

	+ removes margin and padding from an element

+ %row

		@extend %row;

	+ creates an element that completely fills its container

+ %center-block

		@extend %center-block;

	+ centers an element horizontally
	+ only works on elements with a definted width rule	

### Page Element Utilities

+ %info-block

		@extend %info-block;

	+ creates a horizontally centered box that takes up 90% of its container
	+ text is centered

+ %feature-heading

		@extend %feature-heading;

	+ heading for feature boxes	

### Shapes Utilities

### Navigation Utilities

### Effects Utilities

+ solid-drop-shadow

		@include solid-drop-shadow($color);

	+ Applies a solid 2px drop shadow to an element

+ background-transparent

		@include background-transparent($color, $opacity);

	+ Creates a slightly transparent background with a hex color backup
	+ Default opacity of 0.7

+ border-transparent

		@include border-transparent($color, $thickness, $opacity);

	+ Creates a slightly transparent border with a hex color backup
	+ Accepts a hex color value and pixel value for border-width
	+ Default thickness of 5px
	+ Default opacity of 0.7

+ stitched-box

		@include stitched-box($color, $stitch-color, $border-radius, $border-color, $opacity);

	+ Creates an element with a stitched border effect
	+ Takes an optional border and opacity argument

+ stitched-row

		@include stitched-row($color, $stitched-color, $border-color, $opacity);

	+ Creates a stitced top and bottom border
	+ Takes an optional border and opacity argument	