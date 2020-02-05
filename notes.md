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

## Project 4

---

### .filter()

_Filter_ works by passing it a function. That function will loop over every item in an Array. The parameter passed to the function is used to decide wether or not you want to keep the item or not.

- Trick to displaying Arrays or Objects is using _console.table()_ instead of _console.log()._

### .map()

_Map_ takes in an Array, it does something with that Array, then returns a _NEW_ array, but of the same length.

### .sort()

_Sort_ works by taking in a function with 2 arguments, and if, for example _a > b_, then you return either 1, or -1.

### .reduce()

What _reduce_ does is, allow you to build something, on each element.
**Remember** to initialize your count variable after the code block.

You can call querySelectors again any existing DOM element.

```js
const category = document.querySelector('.mw-category');
const links = category.querySelectorAll('a');
```

**Remember**
querySelector will return a _NodeList_
There are a couple ways to turn a NodeList into an array.

const links = Array.from(category.querySelectorAll('a'));

**OR**

const links = [...category.querySelectorAll('a')];

The _Spread_ operator will take every item _out_ of something, (an iterable), and return it back into the containing array.
