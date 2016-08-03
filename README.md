# jQuery-toast
Materialize's toast redone for standalone jQuery

## Usage
**toast** has 5 overloads:

- `toast(options);`
- `toast(message);`
- `toast(message, duration);`
- `toast(message, duration, className);`
- `toast(message, duration, className, completeCallback);`

And the following parameters:

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| options | object `{}` | `{ message: "", duration: 5000, className: "", completeCallback: $.noop  }` | Options to be used by toast |
| message | string `""` or DOM node `<div>` or jQuery object`$()` | `""` | The message or element to show inside the new toast |
| duration | number `0` | 5000 | How long will the toast float before animating out |
| className | string `""` | `""` | Classes to add to the new toast node |
| completeCallback | `function(){}` | `$.noop` | Function to execute after toast animates out |

The `options` parameter has 4 properties, which are equal to the other parameters in every way.

**toast will not show (silently) if no message is provided!**

## Mobile friendly
Hammer.js is automatically supported, just like in Materialize!<br>
All you need to do is add Hammer.js to your project before toast.js and you will be able to "pan" and "swipe" every toast.
