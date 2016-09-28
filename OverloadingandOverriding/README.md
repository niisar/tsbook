### Overloading and Overriding

#### Function Overloading

Function Overloading is 2 or more function with same name but different parameter.

Example: 
```ts
class student{
    Foo(value : string ) : void {};
    Foo(value : number) : void {};
    Foo(value : number, value2 : string) : void {};
    Foo(value2 : string, value : number) : void {};
}
```
In the above example Foo function overloaded to support both string and number parameter.

####Function Overriding

Function Overriding is creating a function in a subclass with the same name as the function in the base class but with different functionality. 

Example:

```ts
class Parent{
    constructor() {}
    Foo(value : any) {}
}
class Child extends parent{
    constructor() { super(); }
    Foo(value : any ) {}
}
```
In the above example we are overriding a base class function Foo in a subclass function. Now we can do different operations in both the functions.