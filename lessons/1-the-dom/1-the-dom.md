# The DOM

## What is the DOM?

The document object model (DOM) is the interface between a site's document (ex. HTML) and scripts (ex. javascript).
In practice the `Document` is a javascript interface that represent the currently loaded document in the web browser.

The global `document` is an implementation of the `Document` interface and provides methods to manipulate the document's nodes (elements)

Some examples of document methods:

```html
<html lang="en">
  <head>
    <title>getElementById example</title>
  </head>
  <body>
    <label id="input-label" for="username-input">Username</label>
    <input name="username" />
  </body>
</html>
```

```js
let labelElement = null;
let inputElement = null;

// these are 2 ways to select the label element
labelElement = document.getElementById("input-label");
labelElement = document.querySelector("#input-label");

// these are 2 ways to select the input element
const [firstInputElement, ...allOtherInputElements] =
  document.getElementsByTagName("input");
inputElement = document.querySelector("input[name='username']");
```

## Exercise - Select box color

Create a web application that does the following:

- [ ] Renders a `div` element of width 300 pixels, height of 300 pixels with a black border of 1 pixel
- [ ] Renders an `input` of type `color` with a `label` 'Color'
- [ ] Renders a `button` with text 'Set color'
- [ ] When the user clicks on the 'Set color' button, the `div` element changes its background color to the color set in the `input`

### Keywords to google

Googling makes you go further...
These are some keywords that might help you with your exercise

- _html color input element_
- _inline element styles_
- _how to handle a button click in javascript_
- _how to read the value of an input element_
- _how to set style of element in javascript_

As a last resort, if you get stuck see `solution.html`
