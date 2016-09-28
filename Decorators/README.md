### Decorator

 Decorators are functions, but a special kind of them. Decorators can used on classes, Methods, properties, and parameters. The best part is that you can write a decorator once and use it on many classes.



 Example: Simplified Angular 2 component decorator



 ```ts
@Component({
 template: '<h1>Hello this is {{title}}</h1>',
})
export class AppComponent {
 title = 'My app!';
}
 ```

 In the Above example AppComponent is a normal class with a ```title``` property, and it has a Component decorator above it. Because the Component decorator is above the class, it works with that class. Here it's defining a view for the AppComponent class, which data binds to the title property of the class. The Component decorator itself is a function.



 You can write decorators yourself, as well. The function takes the object involved, the instance of the class it's above, and a configuration object as a parameter. It uses that information to do something with the object passed in.



 We have got three basic type of decorator in typescript:



 ####Property Decorators

 ####Method Decorators

 ####Class Decorators

 ####Parameter Decorators




