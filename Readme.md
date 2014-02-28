*This repository is a mirror of the [component](http://component.io) module [ianstormtaylor/css](http://github.com/ianstormtaylor/css). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ianstormtaylor-css`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# css
  
  Simple CSS manipulation.

## Installation

    $ component install ianstormtaylor/css

## Example

```js
var css = require('css');
var div = document.getElementById('header');

// get
css(div, 'position'); // "relative"

// set one at a time
css(div, 'position', 'fixed');

// set many at a time
css(div, {
  position: 'fixed',
  top: '24px'
});

// use dashes if you want
css(div, 'font-size', '16px');

// you can omit "px" and it will be added automatically
css(div, 'font-size', 16);
```

## API

### css(el, property)
  
  Get the current value of a CSS `property` of an `el`.

### css(el, property, value)

  Set the `value` of a CSS `property` on an `el`.

### css(el, properties)

  Set the value of a dictionary of `properties` on an `el`.

## License

  MIT
