FFW Grid Components
-------------------
**Author**: Alexander Zizzo, **Date**: 1/27/2014

### General Notes

All section's inner element should be wrapped by a container class. The grid is fluid, meaning it uses percentages. `padding` is favored over `margin` for gutter spaces. Often items an `.inner` or `.content` class will be needed, as is the nature of the global `box-sizing:border-box` selector.


### Grid Classes

> Container classes

All content must be in either of two containers:

* `container-full` - full width (100%) container.
* `container` - a container that is responsive to media queries
	* 960px - Desktop
	* 768px - Tablet
	* 420px - Mobile Landscape
	* 300px - Mobile Portrait
	
	
> Column Classes

* `row` will clear floats, and gives a bottom margin (~20px).
* `span1 - span12` i.e. `span6` is 50%, `span12` 100% width, etc.
* All elements should utilitize these column classes for graceful 'collapsing' into mobile/tablet viewports.

> Box Classes

the `box` class is simply a box shaped css element. it inherits properties from other classes, such as:

 * `box-third` - use for three boxes in a row
 * `box-fourth` - use for four boxes in a row
 * `has_footer` - use when the box has footer element (see *Staff* page)
 * `has_hover_overlay` - applies the hover attribute to the box element

> Buttons

The default button class is `btn`. The colors coincide with the color variables set in `_config.scss`, priortized as **Primary**, **Secondary**, **Tertiary**, **Quaternary**, etc - depending on how many colors the particular site scheme has. Some button class examples are:
    
 * `btn` (defaults to the `primary` color ) 
 * `btn primary transparent`
 * `btn secondary`
 * `btn tertiary large`
    
- For more understanding of buttons, refer to `_buttons.scss`, which utilizes mixins from the `_ffw.scss` mixin library.

> Icons

Icons use the [Font Awesome](http://fortawesome.github.io/Font-Awesome/cheatsheet/) font. Their glyphs are given semantic class names in `_icons.scss`. They leverage CSS3's pseudo classes (`:before`). For example, you can give an achor tag an icon of a heart with the following markup:

 * `<a href="#" class="btn secondary transparent icon icon-heart">Link</a>`




