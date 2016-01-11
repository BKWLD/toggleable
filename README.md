# Toggleable

Show and hide elements when other elements are clicked

## API

- **map(array mapping)**

	Provide a mapping of elements to OTHER elements that should be shown when clicked. `mapping` is an array of objects that look like: `{ on: $el, show: $el}`.  When the on $el is clicked, all the `show` $elements but the one in the pairing are hidden.

## Examples

```js
require('toggleable').map([
	{ on: $('.one'), show: $('other') },
	{ on: $('.two'), show: $('another') }
]).showFirst();
```
