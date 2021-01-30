<!-- Please do not edit this file. Edit the `blah` field in the `package.json` instead. If in doubt, open an issue. -->








[![set-or-get](http://i.imgur.com/EsztPQ4.png)](#)











# set-or-get

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Ask me anything](https://img.shields.io/badge/ask%20me-anything-1abc9c.svg)](https://github.com/IonicaBizau/ama) [![Version](https://img.shields.io/npm/v/set-or-get.svg)](https://www.npmjs.com/package/set-or-get) [![Downloads](https://img.shields.io/npm/dt/set-or-get.svg)](https://www.npmjs.com/package/set-or-get) [![Get help on Codementor](https://cdn.codementor.io/badges/get_help_github.svg)](https://www.codementor.io/johnnyb?utm_source=github&utm_medium=button&utm_term=johnnyb&utm_campaign=github)

<a href="https://www.buymeacoffee.com/H96WwChMy" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png" alt="Buy Me A Coffee"></a>







> Sets or gets an object field value.

















## :cloud: Installation

```sh
# Using npm
npm install --save set-or-get

# Using yarn
yarn add set-or-get
```













## :clipboard: Example



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











## :question: Get Help

There are few ways to get help:



 1. Please [post questions on Stack Overflow](https://stackoverflow.com/questions/ask). You can open issues with questions, as long you add a link to your Stack Overflow question.
 2. For bug reports and feature requests, open issues. :bug:
 3. For direct and quick help, you can [use Codementor](https://www.codementor.io/johnnyb). :rocket:





## :memo: Documentation


### `SetOrGet(input, field, def)`
Sets or gets an object field value.

#### Params

- **Object|Array** `input`: The cache/input object.
- **String|Number** `field`: The field you want to update/create.
- **Object|Array** `def`: The default value.

#### Return
- **Object|Array** The field value.














## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects
I open-source almost everything I can, and I try to reply to everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:


 - Starring and sharing the projects you like :rocket:
 - [![Buy me a book][badge_amazon]][amazon]—I love books! I will remember you after years if you buy me one. :grin: :book:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)


Thanks! :heart:
















## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:

 - `lien`
 - `count-words`
 - `bloggify-flexible-router`
 - `bloggify-template-renderer`
 - `svg.connectable.js`
 - `engine-parser`
 - `engine-builder`
 - `enny`
 - `bloggify-mongoose`
 - `bloggify-shop`
 - `bloggify-theme-renderer`











## :scroll: License

[MIT][license] © [Ionică Bizău][website]






[license]: /LICENSE
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
[badge_patreon]: https://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: https://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: https://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: https://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
