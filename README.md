#jQuery-ui-Slider-Pips
  
###Plugin for adding little 'pips' and labels to a jQuery UI slider widget.      
  
  
This plugin **extends** the [jQuery UI Slider widget](http://jqueryui.com/slider/).    

check out the Demo / Docs:  
http://simey.me/projects/jquery-ui-slider-pips/

------------------------------------  
  
###Requirements:
  - jQuery (1.9+)
  - jQuery UI (1.10+)
  - A Reason to use it
  
------------------------------------  
  
###Usage:   
Include the plugin javascript file after jquery-ui.   
Include the CSS file, edit as you please.  
  
  
```javascript  
// First of all attach a slider to an element.
$('.element').slider({opts});

// Then you can give it pips and labels!
$('.element').slider('pips', {    
    first: 'label',
    last: 'label',  
    rest: 'pip',
    labels: ['label1', 'label2', ...],
    prefix: "",
    suffix: ""
});
  
// And finally can add floaty numbers (if desired)
$('.element').slider('float', {    
    handle: true,
    numbers: true,
    prefix: "",
    suffix: ""  
});

// methods can (and probably should) be chained:
$('.element').slider().slider('pips').slider('float');
```

#####Pips method takes the options: `first, last, rest` with the values of:  
- `"pip"` - adds a pip. (default for `rest`)    
- `"label"` - adds a pip and a number. (default for`first` & `last`)   
- `false` - hides the number and pip.  
  
#####Pips method also can have option of: `labels` with values of:
- `false` - defaults labels to be numberic value
- `[array]` - array of values to apply to pips

#####Float method takes the options: `handle, numbers` with the values of:  
- `true` - adds floaty number. (default)    
- `false` - no floaty number.

#####Pips and Float methods both take the options: `prefix, suffix` with the values of:  
- `""` - no prefix/suffix. (default)    
- `"prefix"` - a string prefixed/suffixed.
  
  
------------------------------------

###Customisation:  
All customisation should be done to the CSS file, or in your own CSS.  
The base styles I've provided do a decent job in the Demo,   
but they will need tweaking to suit your needs and UI theme.  
  
------------------------------------

###Compatibility:   
Modern Browsers, IE7+   
_(will need some CSS work for IE7 display issues, I'm not interested in doing them :P)_

------------------------------------

###License:  
Open Source MIT.  
http://opensource.org/licenses/MIT


------------------------------------

###Changlog:  

- **Nov 22, 2013** - CSS Changes
  - [Fix tiny bit of JS for vertical sliders](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/e7da19e5489c43ae2d439165199904812ee2e07f)
  - [Add missing CSS for vertical floats](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/d8ad4da1392f79f962b71aa842afee687d48ab57)

***

- **Aug 28, 2013** - Update to `1.2`
  - Convert to a grunt/node setup
  - Clean up code with jshint
  - Remove legacy demo

***

- **June 20, 2013** - Update to `1.1`
  - [Add ability to `prefix` and `suffix` labels and floats](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/cd483265a458ad1a3f200f16e4518a7f3d3db27a) - thanks [Xeeeveee](https://github.com/xeeeveee)
  - [Fix some bugs, clean up code](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/fda25f8545c941480fd10e6eb22e8efe91a78128)
  - update demo to show new features

***

- **March 13, 2013** - Update to `1.0`
  - [Add ability to create custom labels with an array](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [Change `number` option to `label`](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [Add `labels` option](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [CSS style names changed to reflect update `ui-slider-pip-value`, `ui-slider-value` .. etc](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L0L7)
  - fix various typos  
  
***

- **March 10, 2013** - Update to `0.2`
  - [Added extension for 'floating' numbers](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/aeacad87d47d79a96b9f26d2d83a5c3206d9f90f)
  - [Fixed so that sliders can start with negative numbers](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/aeacad87d47d79a96b9f26d2d83a5c3206d9f90f)

------------------------------------  
