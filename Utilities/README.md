### Arrow Function and Template String

Fat arrow function also called as lambda function. Fat arrow function is shorthand for function, automatically capture this and arguments.

Example: **Typescript**
```ts
var data: string[] = ['Rahul', 'Ram', 'Jia'];
data.forEach( (line) => console.log(line) );
```

Example: **JavaScript**
```js
var data = ['Rahul', 'Ram', 'Jia'];
data.forEach(function(line) { console.log(line); });
```

### Template strings

  Template strings are the strings that use back-ticks like (`). Template strings are mainly used for Multi Line String and String Interpolation.

Example: **Typescript**
```ts
var story= `Lorem ipsum sit amet, 
 quod veritus consectetuer ex.`;
```

Example: **JavaScript**
```js
var story= 'Lorem ipsum sit amet, \
\n quod veritus consectetuer ex.';
```
---
Example: **String Interpolation in Typescript**
```ts
var story= 'Lorem ipsum sit amet';
var html = `<div>${story}</div>`;
```
Example: **String Interpolation in JavaScript**
```js
var story = 'Lorem ipsum sit amet';
var html = '<div>' + story + '</div>';
```