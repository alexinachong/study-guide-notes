# Frontend

## JavaScript | Prototypes (W1D1)

### Give a high level overview of what an object's prototype represents.

An object's prototype is the template object from which it inherits. ([Object Prototypes](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes))

### What are the differences between the `__proto__` and `prototype` attributes?

The `__proto__` attribute is an accessor property of `Object.prototype` object. It exposes the internal prototype linkage of an object through which it is accessed. ([JavaScript Inheritance](https://hackernoon.com/understand-nodejs-javascript-object-inheritance-proto-prototype-class-9bd951700b29))

`__proto__` is the actual object that is used in the lookup chain to resolve methods, etc. `prototype` is the object that is used to build `__proto__` when you create an object with `new`. `prototype` is the blueprint for `__proto__`. ([`__proto__` vs `prototype`](https://stackoverflow.com/questions/9959727/proto-vs-prototype-in-javascript))

### What happens when we do or don't explicitly set an object's prototype?

### What is an object's default prototype?

### What are the valid values for an object's prototype?

## JavaScript | Closures (W1D2)

### What are the benefits of a Javascript closure?

Closures allow data encapsulation.

### Formally define a Javascript closure.

A closure is the combination of a function and the lexical environment from which it was declared. Closure allows a function to access variables from an enclosing scope - environment - even after it leaves the scope in which it was declared.

### Give an example of a closure.

### What is data encapsulation?

## JavaScript | ES5 vs ES6

### Discuss 4 differences between ES5 and ES6 that you find important.

1.  ES5 only had function-level scope (i.e., wrapping code in functions to create scope), whereas ES6 has block-level scope (i.e., using curly braces to create scope) when we use `let` or `const`, instead of `var`. This prevents variable-hoisting outside of the given scope.
2.  In ES5, `this` can vary based on where and how it is called. ES6 supports a lexical `this` (by way of a fat arrow function), which forces the variable `this` to always point to the object within which it is physically located.
3.  In ES5, arguments are array-like, so we can loop over them, but cannot use Array functions (like `sort`, `slice`, etc.) on them. However, in ES6, we can use "rest" parameters (represented as `...args`, as in `const mySort = (...args) => { args.sort }`), which is in array, and thus permits us to use Array functions.
4.  Whereas strict mode (`use strict`) was optional in ES5, it is necessary for many ES6 features. Babel automatically adds `use strict` at the top of the file, which helps us identify common issues in our code and forces us to write better JavaScript.

## HTML5 | Media Queries (W1D1)

### Name 5 benefits of HTML5.

1.  Accessibility
2.  Video and Audio Support
3.  Game Development
4.  Legacy/Cross Browser Support
5.  Mobile Responsiveness

### What is `localStorage`? How might you use it?

`localStorage` is a cross between cookies and a client-side database. It's better than cookies because it allows for storage across multiple windows, it has better security, and performance and data will persist even after the browser is closed. This allows you to load the user's previous application state.

### Why are media queries useful?

Media queries allow us to set conditions on our CSS so that pages display differently depending on what conditions are true about the viewing window.

### What is mobile-first design? Be as specific as possible.

Mobile-first design is the practice of designing for mobile before designing for desktop or other devices. This is a popular practice because it is easier to scale your design up than scale down.
