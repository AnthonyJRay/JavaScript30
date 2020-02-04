# JavaScript30 By: Wes Bos

## Project 1

If you use _.play()_ on an audio element, it waits for the audio to finish before being able to play again.

When you have an Array of elements, you cannot attach an EventListener to it. You must instead loop through the Array and attach an EventListener to each individual element.

JavaScript has a 'transitionend' you can use in an Event Listener, to control elements under the conditions of when it's transition has finished.

## Project 2

transform-origin changes where the pivot point it. By default it is set to 50%.
100% = Right Side
0 = Left Side

## Project 3

CSS Variables can be changed with JavaScript. Whereas with SASS, variables are set at compile time.

Declaring CSS variables uses ( -- ).

```css
:root {
  --spacing: 10px;
}
```

To use CSS variables, you assign them with var.

```css
img {
  padding: var(--spacing);
}
```

querySelectorAll returns an Array-like Object. It looks like an Array, but it is a _NodeList_

The difference between an Array and a NodeList is the _Methods_ available for them.

_NodeList's do not have access to many of the methods Arrays do._

You _can_ convert NodeList's to Arrays if needed.
