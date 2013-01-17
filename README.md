# jQuery.wigglesticks

### About

Wigglesticks extends [jQuery.Stickem](https://github.com/davist11/jQuery-Stickem)

It allows taller-than-viewport sticky content to scroll independently while remaining stuck. 

This means that as you scroll down the page, the sticky content remains still until you reach its bottom, at which point it sticks to the bottom of the viewport, and vice-versa for the top of the content. The sticky content is bounded on the top and bottom by its container, and won't leave those boundaries.

### To Use

* copy stickem.js and wigglesticks.js somewhere into your project
* link to jquery, stickem.js, and wigglesticks.js in that order in your &lt;head&gt;
* on page load, call the wigglesticks function on the element which you want to sticky scroll. Make sure this element has a parent around itself and its sibling content.

```javascript
$(function() {
  $('.wiggle-content').wigglesticks();
});
```

### Options

You can currently set the item's selector, its parent's selector, and the container around them both.

These values currently default, respectively, to the item on which you call the function, that item's parent, and '.container'.

Here's an example of overriding the default values:

```javascript
$(function() {
  $('.wiggle-content').wigglesticks({
    'item'      : '.wiggle-content-alternative',
    'parent'    : '.wiggle-content-parent',
    'container' : '.container-alternative'
  });
});
```

Check back or "star" for updates! Create an issue if you have any ideas.
