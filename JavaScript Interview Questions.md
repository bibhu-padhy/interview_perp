# JavaScript Interview Questions - Beginner to Advanced

## **FUNDAMENTALS & BASICS**

### Data Types & Variables
- What are the primitive data types in JavaScript?
- Difference between `var`, `let`, and `const`?
- What is hoisting?
- What is the Temporal Dead Zone?
- What happens when you declare a variable without `var`, `let`, or `const`?
- What is the difference between `null` and `undefined`?
- What is `typeof` operator and its edge cases?
- What is type coercion in JavaScript?
- What are falsy values in JavaScript?
- What is the difference between `==` and `===`?

### Functions
- What is function hoisting?
- Difference between function declaration and function expression?
- What are arrow functions and how do they differ from regular functions?
- What is the `arguments` object?
- What are rest parameters and spread operator?
- What is a higher-order function?
- What are pure functions?
- What is function currying?
- What is partial application?
- What are IIFE (Immediately Invoked Function Expressions)?
- What is the difference between `call`, `apply`, and `bind`?

### Scope & Context
- What is lexical scoping?
- What is the scope chain?
- What is the execution context?
- What is the `this` keyword and how does it work?
- How does `this` behave in arrow functions?
- What is the global object?
- What are closures?
- What are the practical uses of closures?
- What is the module pattern?

## **OBJECTS & ARRAYS**

### Objects
- How do you create objects in JavaScript?
- What is object literal notation?
- What are getters and setters?
- What is `Object.create()`?
- What is prototypal inheritance?
- What is the prototype chain?
- What is `__proto__` vs `prototype`?
- What are constructor functions?
- How do you check if a property exists in an object?
- What is `hasOwnProperty()`?
- What are property descriptors?
- What is `Object.defineProperty()`?
- What is `Object.freeze()`, `Object.seal()`, and `Object.preventExtensions()`?
- How do you clone objects (shallow vs deep)?
- What is object destructuring?

### Arrays
- What are different ways to create arrays?
- What is the difference between `Array.from()` and `Array.of()`?
- What are array-like objects?
- How do you convert array-like objects to arrays?
- What is the difference between `forEach`, `map`, `filter`, `reduce`?
- What is the difference between `find` and `findIndex`?
- What is the difference between `some` and `every`?
- What is array destructuring?
- How do you flatten nested arrays?
- What is the difference between `sort()` and `toSorted()`?
- What is the difference between `reverse()` and `toReversed()`?
- What is the difference between `splice()` and `slice()`?

## **ASYNCHRONOUS JAVASCRIPT**

### Callbacks & Promises
- What is the event loop?
- What is the call stack?
- What is the callback queue?
- What are callbacks?
- What is callback hell?
- What are Promises?
- What are the states of a Promise?
- What is Promise chaining?
- What is `Promise.all()`, `Promise.race()`, `Promise.allSettled()`?
- What is `Promise.any()`?
- What is the difference between `Promise.resolve()` and `Promise.reject()`?

### Async/Await
- What is async/await?
- How do you handle errors with async/await?
- What is the difference between Promises and async/await?
- Can you use async/await with forEach?
- How do you run async operations in parallel vs sequential?

### Timers
- What is `setTimeout` and `setInterval`?
- What is `clearTimeout` and `clearInterval`?
- What is the minimum delay for `setTimeout`?
- What is `requestAnimationFrame`?

## **ERROR HANDLING**

- What are the types of errors in JavaScript?
- What is `try...catch...finally`?
- How do you create custom errors?
- What is error propagation?
- How do you handle errors in Promises?
- How do you handle errors in async/await?
- What is the `Error` object?

## **ES6+ FEATURES**

### Modern Syntax
- What are template literals?
- What is the spread operator?
- What is the rest operator?
- What is array/object destructuring?
- What are default parameters?
- What is the `for...of` loop?
- What is the `for...in` loop?
- What are computed property names?
- What is shorthand property notation?

### Classes
- What are ES6 classes?
- What is the `constructor` method?
- What are static methods?
- What is inheritance with `extends`?
- What is `super` keyword?
- What are private fields and methods?
- What are getters and setters in classes?

### Modules
- What are ES6 modules?
- What is `import` and `export`?
- What are named exports vs default exports?
- What is dynamic import?
- What is the difference between CommonJS and ES6 modules?

### New Data Structures
- What is `Map` and how is it different from Object?
- What is `Set` and its methods?
- What is `WeakMap` and `WeakSet`?
- What are `Symbol` and its use cases?
- What is `BigInt`?

## **ADVANCED CONCEPTS**

### Memory Management
- How does garbage collection work in JavaScript?
- What are memory leaks and how to prevent them?
- What are weak references?
- What is reference counting?

### Performance
- What is debouncing?
- What is throttling?
- What is memoization?
- What is lazy loading?
- What are Web Workers?
- What is the difference between `defer` and `async`?

### Functional Programming
- What is functional programming?
- What are first-class functions?
- What is function composition?
- What are monads?
- What is immutability?
- What are pure functions vs impure functions?

### Design Patterns
- What is the Singleton pattern?
- What is the Observer pattern?
- What is the Factory pattern?
- What is the Module pattern?
- What is the Revealing Module pattern?
- What is the Prototype pattern?
- What is the Command pattern?

## **BROWSER APIS & DOM**

### DOM Manipulation
- What is the DOM?
- What is the difference between `getElementById`, `querySelector`, and `querySelectorAll`?
- What is event bubbling and capturing?
- What is event delegation?
- How do you prevent default behavior?
- What is `stopPropagation()` vs `stopImmediatePropagation()`?
- What are synthetic events?
- What is the difference between `innerHTML`, `textContent`, and `innerText`?
- What is `DocumentFragment`?

### Browser Storage
- What is localStorage vs sessionStorage?
- What are cookies?
- What is IndexedDB?
- What is the Cache API?

### Network & APIs
- What is the Fetch API?
- What is XMLHttpRequest?
- What are HTTP status codes?
- What is CORS?
- What is JSONP?
- What are WebSockets?
- What is Server-Sent Events (SSE)?

## **ADVANCED JAVASCRIPT CONCEPTS**

### Metaprogramming
- What is `Proxy` object?
- What is `Reflect` API?
- What are property descriptors?
- What is `Object.defineProperty()`?
- What are symbols and their use cases?

### Generators & Iterators
- What are generators?
- What is the `yield` keyword?
- What are iterators?
- What is the iterator protocol?
- What is `Symbol.iterator`?
- What are async generators?

### Regular Expressions
- What are regular expressions?
- What are regex flags?
- What are capturing groups?
- What are lookaheads and lookbehinds?
- What is the difference between `test()`, `exec()`, `match()`, `search()`?

### Advanced Async Patterns
- What are async iterators?
- What is `AbortController`?
- What are Observables?
- What is reactive programming?

## **TESTING & DEBUGGING**

### Debugging
- How do you debug JavaScript code?
- What are breakpoints?
- What is the debugger statement?
- What are source maps?
- What is console API methods?

### Testing Concepts
- What is unit testing?
- What is integration testing?
- What is Test-Driven Development (TDD)?
- What is mocking?
- What are stubs and spies?

## **SECURITY**

- What is XSS (Cross-Site Scripting)?
- What is CSRF (Cross-Site Request Forgery)?
- What is Content Security Policy (CSP)?
- What is same-origin policy?
- How do you sanitize user input?
- What is eval() and why is it dangerous?

## **PERFORMANCE & OPTIMIZATION**

### Performance Monitoring
- What are performance APIs?
- What is `performance.now()`?
- What is the Performance Observer API?
- What are Core Web Vitals?

### Code Optimization
- What is tree shaking?
- What is code splitting?
- What is lazy loading?
- What is preloading vs prefetching?
- What is critical rendering path?

## **TYPESCRIPT INTEGRATION**

- What is TypeScript?
- What are types vs interfaces?
- What are generics?
- What is type assertion?
- What are union and intersection types?
- What are decorators?
- What is type narrowing?

## **FRAMEWORK-AGNOSTIC CONCEPTS**

### State Management
- What is state management?
- What is unidirectional data flow?
- What is the Flux pattern?
- What is immutable state?

### Component Architecture
- What are components?
- What is component composition?
- What are higher-order components?
- What is dependency injection?

## **NODE.JS FUNDAMENTALS** (if applicable)

- What is Node.js event loop?
- What are streams in Node.js?
- What is the difference between process.nextTick() and setImmediate()?
- What is clustering in Node.js?
- What are child processes?

## **CODING CHALLENGES & ALGORITHMS**

### Array Problems
- Implement array methods (map, filter, reduce) from scratch
- Find duplicates in an array
- Rotate an array
- Merge sorted arrays
- Two sum problem
- Maximum subarray sum

### String Problems
- Reverse a string
- Check if string is palindrome
- Find longest substring without repeating characters
- Implement string compression
- Anagram detection

### Object Problems
- Deep clone an object
- Flatten nested objects
- Merge objects
- Compare two objects for equality
- Implement object.assign from scratch

### Function Problems
- Implement call, apply, bind from scratch
- Implement debounce and throttle
- Implement memoization
- Implement function composition
- Implement partial application

### Promise Problems
- Implement Promise from scratch
- Implement Promise.all, Promise.race
- Chain multiple async operations
- Implement retry mechanism
- Implement timeout for promises

### Data Structure Implementation
- Implement Stack and Queue
- Implement LinkedList
- Implement Binary Tree traversal
- Implement Hash Table
- Implement Trie

### Design Problems
- Design a event emitter
- Design a pub-sub system
- Design a cache with LRU eviction
- Design a rate limiter
- Design a simple router

## **SYSTEM DESIGN (Frontend Focus)**

- How would you design a frontend architecture?
- How do you handle state management in large applications?
- How do you implement caching strategies?
- How do you handle real-time updates?
- How do you optimize bundle size?
- How do you implement micro-frontends?

## **BROWSER INTERNALS**

- How does JavaScript engine work?
- What is JIT compilation?
- What is the V8 engine?
- How does browser parsing work?
- What is the critical rendering path?
- How do you optimize rendering performance?

## **EDGE CASES & GOTCHAS**

- What happens when you compare NaN?
- What is the result of 0.1 + 0.2?
- What is the typeof null?
- What happens with automatic semicolon insertion?
- What are the quirks with sort() method?
- What happens with parseInt() edge cases?
- What is the banana operator ()?
- What are the edge cases with this binding?
