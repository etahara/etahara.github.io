---
layout: project
type: project
image: img/projects/Jamba_juice.png
title: "Jamba Juice Menu"
date: 2023
published: true
labels:
  - Javascript

summary: "My first experience with classes and constructors in Javascript"
---

<img width="400px" class="text-center rounded float-start pe-4" src="../img/projects/jambajuicemenu.jpg">

Javascript is a scripting language created by Brendan Eich in 1995 that was originally used for the Netscape Navigator web browser. In my ICS 314 class we use it as a means to study software engineering and to create short programs to experience programming. 

In one of our practice assignments we were asked to create a program revolving around a Jamba Juice menu through the use of classes and constructor. This was a very useful, albiet confusing, assignment to properly learn this concept as foods and drinks have many different components that need to be accounted for when eating and ordering them. I think the most outstanding part of this was understanding the concept of how objects can be comprised of other objects attatched to it, as each drink had a name, a list of ingredients, a corresponding price per size, and calorie count per size. Although this concept may seem elementary, as we know that everything in this world is comprised of other things down to a microbial level, but the methods of referring to each derived object and the functions using them were a bit confusing to grasp.

I think creating a menu based project to learn class and constructors was a very smart decision by my professor, as it's a very simple process to learn as it's something we have to think about everytime we want to order something. The class and constructor is something that we can apply to many other topics such as jobs, mobs in video games, or how our simple computer works. It was a confusing process to learn but I think by doing this I have a greater understanding of how class and constructors work and how I can apply it to other obejcts.

Here is some code to illustrate the constructor, an example class, and the test functions and the output
```
class MenuItem {
  constructor(name, ingredients, price, calories) {
    this.name = name;
    this.ingredients = ingredients;
    this.price = price;
    this.calories = calories;

  }
}

class Menu {
  constructor() {
    this.menuItems = [];
  }

  addMenuItem(menuItem) {
    this.menuItems.push(menuItem);

  }
```

```
const PapayaSunrise = new MenuItem("Papaya Sunrise", ["papaya", "strawberry", "peach"], [5.15, 5.75, 6.55], [190, 280, 330]);
const PeachPerfection = new MenuItem("Peach Perfection", ["peach", "mango", "strawberry"], [5.15, 5.75, 6.55], [210, 320, 360]);
const StrawberryDragon = new MenuItem("Strawberry Dragon", ["pitaya", "strawberry", "orange", "passionfruit", "mango", "banana"], [5.85, 6.25, 6.85], [360, 480, 610]);
const StrawberryWhirl = new MenuItem("Strawberry Whirl", ["strawberry", "banana", "apple"], [5.15, 5.75, 6.55], [210, 310, 380]);

const myMenu = new Menu();
myMenu.addMenuItem(PapayaSunrise);
myMenu.addMenuItem(PeachPerfection);
myMenu.addMenuItem(StrawberryDragon);
myMenu.addMenuItem(StrawberryWhirl);

console.log(myMenu);
```

```
{
  menuItems: [{
  calories: [190, 280, 330],
  ingredients: ["papaya", "strawberry", "peach"],
  name: "Papaya Sunrise",
  price: [5.15, 5.75, 6.55]
}, {
  calories: [210, 320, 360],
  ingredients: ["peach", "mango", "strawberry"],
  name: "Peach Perfection",
  price: [5.15, 5.75, 6.55]
}, {
  calories: [360, 480, 610],
  ingredients: ["pitaya", "strawberry", "orange", "passionfruit", "mango", "banana"],
  name: "Strawberry Dragon",
  price: [5.85, 6.25, 6.85]
}, {
  calories: [210, 310, 380],
  ingredients: ["strawberry", "banana", "apple"],
  name: "Strawberry Whirl",
  price: [5.15, 5.75, 6.55]
}]
}
```

[Source](http://courses.ics.hawaii.edu/ics314s23/morea/javascript-2/experience-jamba-juice-1.html)
