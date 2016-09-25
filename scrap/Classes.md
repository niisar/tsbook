### Classes in Typescript

Classes an Objected Oriented Style of programming. Object Oriented preferred for building large scale app. Typescript like other Object Oriented programming includes features. Features like inheritance, abstract classes, interface, setter-getter and more.

Example:

```ts
class Menu {
 // Properties
  items: Array<string>;
  pages: number;
  // A constructor
  constructor(item_list: Array<string>, total_pages: number) {
    // The this keyword is mandatory.
    this.items = item_list;    
    this.pages = total_pages;
  }

  // Methods
  list(): void {
    console.log("Our menu for today:");
    for(var i=0; i<this.items.length; i++) {
      console.log(this.items[i]);
    }
  }
} 
// Create a new instance of the Menu class.
var sundayMenu = new Menu(["pancakes","waffles","orange juice"], 1);
// Call the list method.
sundayMenu.list();
```