### Typing

Types helps when reading code because it clarifies your intentions, Hear are the Some of the basic types:

```ts
let isDone: boolean = false;
let height: number = 6;
let name: string = "bob";
let list: number[] = [1, 2, 3];
let list: Array = [1, 2, 3];
enum Color {Red, Green, Blue};
let c: Color = Color.Green;
let notSure: any = 4;
notSure = "maybe a string instead";
notSure = false;
```

We can notice `let` keyword used instead of `var` to declare a variable. This is because let allows you to declare variables to a limited scope of block or statement.

`let` is preferable because it reduces the scope in which an identifier is visible.

> Babel's [guide to ES6](https://babeljs.io/docs/learn-es6/#let-const) says:
>
> `let` is the new `var`.

### Function Types

We have function types too

```ts
function add(x: number, y: number): number {
 return x + y;
}
let myAdd = function(x: number, y: number): number { return x+y; };
```

We can add types to each of the parameters and then to the function itself to add a return type.


