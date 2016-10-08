
# Builder Design Pattern 



# Builder Pattern vs Factory method pattern
we usually face when we have to decide when to use factory method pattern and builder pattern. 

A factory is simply a wrapper function around the constructor. The principle difference is that a factory method pattern require the entire object to be built in a single call, will all the parameters pass in on a single line. Then final object will be return.

A real life example can be “meal of the day” in a restaurant. The creation of the meal is a factory pattern, because you tell the kitchen get me the meal of today and the kitchen decide what object to generate based on the hidden criteria.

A builder pattern, whereas is a wrapper object around all the possible parameters you might want to pass to a constructor. This allows you to use setter method to build your own parameter list.

A real life example appears if you order a custom pizza ( any drink). In this case, waiter tell the chef ( TeaBuilder, CoffeeBuilder in our example, you will see soon) I need a pizza; add extra cheese, olives, and corn to it. Therefore, the builder exposes the attributes the generated object should have, but hide how to set them.

* [Code](https://dzone.com/articles/design-patterns-builder)
* [Code](https://www.tutorialspoint.com/design_pattern/builder_pattern.htm)

![](https://myjavalatte.files.wordpress.com/2014/10/b9d61-pizza_builder_patter_example.jpg?w=960)
