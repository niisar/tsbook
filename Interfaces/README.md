###Interface

Interface is one of the confusing terms in OOPs. To understand it let us go through the story below:

> You are in the middle of a large, empty room, when a zombie suddenly attacks you.
You have no weapon.

> Luckily, a fellow living human is standing in the doorway of the room.
>
>"Quick!" you shout at him. "Throw me something I can hit the zombie with!"

>Now consider:
> You didn't specify (nor do you care) exactly what your friend will choose to toss;
> ...But it doesn't matter, as long as:

> * It's something that can be tossed (He can't toss you the sofa)
> * It's something that you can grab hold of (Let's hope he didn't toss a shuriken)
> * It's something you can use to bash the zombie's brains out (That rules out pillows and such)
> 
> It doesn't matter whether you get a baseball bat or a hammer -
> as long as it implements your three conditions, you're good.
> 
> To sum it up:
> 
> When you write an interface, you're basically saying: "I need something that..."  
> [Source](http://stackoverflow.com/a/14244705/2545270)

Interfaces used to type-check whether an object fits a certain structure. When translated to JavaScript, interfaces disappear. Their purpose is to help in the development stage.

Example:

```ts
interface Food {
    name: string;
    calories: number;
}
function eat(food: Food): void{
  console.log("Our " + food.name + " has " + food.calories + " calories.");
}
var ice_cream = {
  name: "ice cream", 
  calories: 200
}
eat(ice_cream);
```