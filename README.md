[![set-or-get](http://i.imgur.com/EsztPQ4.png)](#)

# set-or-get [![Support this project][donate-now]][paypal-donations]

Sets or gets an object field value.

## Installation

```sh
$ npm i set-or-get
```

## Example

```js
// Dependencies
var SetOrGet = require("set-or-get");

// Create an object
var cache = {};

SetOrGet(cache, "foo", []).push(42);
// { foo: [42] }

SetOrGet(cache, "bar", {}).baz = 42;
// { foo: [42], bar: { baz: 42 } }

SetOrGet(cache, "foo", []).push(7);
// { foo: [42, 7], bar: { baz: 42 } }

console.log(cache);
// =>
// {
//   foo: [42, 7]
// , bar: { baz: 42 }
// }
```

## Documentation

### `SetOrGet(input, field, def)`
Sets or gets an object field value.

#### Params
- **Object|Array** `input`: The cache/input object.
- **String|Number** `field`: The field you want to update/create.
- **Object|Array** `def`: The default value.

#### Return
- **Object|Array** The field value.

## How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].

## Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:

 - [`lien`](https://github.com/LienJS/Lien)

 - [`svg.connectable.js`](https://github.com/jillix/svg.connectable.js) by jillix

## License

[KINDLY][license] © [Ionică Bizău][website]

[license]: http://ionicabizau.github.io/kindly-license/?author=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica@gmail.com%3E&year=2015

[website]: http://ionicabizau.net
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md