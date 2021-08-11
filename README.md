# Random Domino Picker

### [View this page live!](https://davegregg.github.io/random-dominoes-demo-beryllium1/)

--- 

Today, we are learning how to search the DOM (the living HTML page as it runs within the browser) for elements and change things about those elements *dynamically.*

##### Key Features:
- `document.querySelector()`
- `document.querySelectorAll()`
- `anyElement.classList.add("any-class-name")`

Along the way, we may also discover a few cool tricks in CSS for adding a lot of visual character to our web page, without a lot of code!:
- __display: none;__ *vs.* __visibility: hidden;__
    - Both rules will make an element "disappear." But one preserves that element's place in the flow of the document. And the other completely removes the element from the flow, as though it does not exist. Which is which?
- __filter: drop-shadow(__`x-axis-offset` `y-axis-offset` `blur-radius` `color`__);__
    - [This rule](https://mdn.io/css-drop-shadow) allows us to add a shadow or glow effect to an element!
    - Example: `filter: drop-shadow(0 0 0.25rem white);` will create a shadow effect, centered along the x-axis (`0`) and the y-axis (`0`). This color for this shadow will be diffused (blurred) across a distance of `0.25rem`. The higher this number, the larger and softer the shadow effect will be. (If this number is too high, you may not be able to see the shadow effect at all.) Finally, this shadow will be `white`, making the "shadow" to work like a "glow" effect.
- __any-selector:hover { }__
    - [This `:hover` pseudo-class selector](https://mdn.io/hover-selector) allows us to apply styles which will only take affect *when the user hovers over the element with their pointer!* Imagine the possibilities.
- __transform: scale(__`some-scaling-factor`__);__
    - [The `transform` property](https://mdn.io/css-transform) allows us to transform an element visually! Among other options, we can `scale()` an element to a different size in a *purely visual* way, without affecting the flow of the document! Compare this to forcing the size of an element to change using other CSS properties.
    - Example: `transform: scale(1.5)` will scale the size of a selected element to 150% of its usual size. That is a total 50% increase in size.
- __transition:__ `some-property-name` `some-duration`__;__
    - [The `transition` property](https://mdn.io/css-transition) allows to chose another CSS property (in this case, `transform`) and apply its effect slowly, over a period of time, rather than instantly.
    - Example: `transition: transform 1s` will apply any `transform` style change for this element over the course of a 1 second.
    - Example: `transition: font-size 0.5s` will apply any `font-size` style change for this element over the course of half a second.

How do you think we can improve or reimagine *this project* once we know how to __add new HTML elements to the page using JavaScript?__ That's what we'll be learning tomorrow: `document.createElement()` and `parentElement.append(newChildElement)`!

How do you think we can improve or reimagine *this project* once we know __better ways to get input from the user?__ That's what we'll be learning next week: HTML forms!
