###Inheritance

  When a new class created from an existing class. Such that new class inherits attributes and behavior of existing class called Inheritance.
  
  
> If you want more information on Inheritance in JavaScript. 
> Look at the Mozilla Developer Network article: [Inheritance and the prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)
  
  Example: In this example we have two classes Employee and Manager as shown below.
  
```ts
class Employee {
    private _name : string;
    constructor(name:string){
       this._name = name;
    }
}
//To create a subclass we use extends
class Manager extends Employee {
    constructor(name:string){
       // To call the base class member we use super
       super(name);
    }
}
```

We are using `super()` to call the base class constructor. In the above example we are passing name into our base class to update the `_name` field in base class. 

Also note that we cannot call a `super()` method if we haven't extended our class from any base class.