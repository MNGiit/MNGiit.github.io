---
layout: post
title:      "JavaScript and the keyword extends"
date:       2020-02-09 04:54:23 +0000
permalink:  javascript_and_the_keyword_extends
---


JavaScript has a keyword called **extends**.  One of the important reasons to use this keyword is to stop code from repeating more than once. A coder doesn't have to repeat the same exact lines of code in different kinds of classes.

Let's say we have a class Home, and class Work. Both Home and Work have addresses, and if we want the classes to have a method that...returns the string of the address, which we'll call printAddress(), it's possible to write this function once, and have both classes use it. That's where the keyword **extends** comes in.

To do this we'll need another class. Since Home and Work are usually in a building of some kind, we'll call it building, or class Building. We then place printAddress() in class Building, and that's it! Well almost. Make sure to extend class Home and class Work as well. It should look something like this:

```
class Building {
  // important things like constructor go here
	// let's not forget printAddress()
	printAddress() {
	  // returns a string
	}
}

class Home extends Building {
  // other code that class Home should have
}

class Work extends Building {
  // other code that class Work should have
}
```

Notice that there's another class, and the other two classes use the extend keyword. When a class extends, it's inheriting code from the other class (the class to the right of the extends). Now let's say we have other things like police station, school, 99 cents shop, pizzeria, and etc that we want to turn into a class. Since they're all structures like a home or work place, then we can have these new classes inherit from class Building and save a ton of time.
