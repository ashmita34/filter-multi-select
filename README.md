# filter-multi-select

A pure-JS implementation of Django's filter_horizontal widget for multiselects.

## Why?

Because Django's *filter_horizontal* turns a nasty, almost unusable multiselect widget
into a cool *two multi-selects with filters that pass shit around with buttons* widget without
any hassle. I wanted it too, but better.

## Better?

Well, not really. It achieves exactly the same, but it has no styles and since it's pure
JavaScript, it doesn't require external libs such a jQuery. It probably performs better too.

## What have you got against jQuery?

Nothing, but I think it's overkill for something so simple. JavaScript has come along way
with its querySelectors and (holy shit!) Promises, so libs are not necessary anymore. Unless
you're doing something super-complex. This is not the case.

## How do I use it?

You include the file `filter-multi-select.js` in your document (`<script type...` you know that,
right?) and then you simply pass the field to its constructor and *start* it, like so:

```
var someField = document.querySelector('#multiselect-field-with-tons-of-options');
MultiSelectField(someField).start();

var anotherField = document.querySelector('#another-multiselect-with-even-more-options');
MultiSelectField(anotherField).start();
```

## Can I help?

Of course. This thing works, but it can probably (read "most definitely") be improved a lot, so
any help will be appreciated.
