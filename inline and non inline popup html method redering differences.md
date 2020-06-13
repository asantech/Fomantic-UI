# Fomantic-UI

In Fomantic-UI, popup can be inline or non line.
Popups have an html() method, in which you can create your custom popup content.

In in an inline popup, the html() method (the code written inside the method) is executed only once.
In a non inline popup, the html() method is executed each time the popup is shown.

If a popup is inline it will be created next to current element, allowing for local css rules to apply. It will not be removed from the DOM after being hidden. 

Otherwise a non inline popup will appended to body and be removed after being hidden.

```
/* JS code */

// inline popup
var popup = $(.element).popup({
  inline: true
})
```
