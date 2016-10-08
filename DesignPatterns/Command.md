
# Command Pattern Important Points
Command is the core of command design pattern that defines the contract for implementation.
Receiver implementation is separate from command implementation.
Command implementation classes chose the method to invoke on receiver object, for every method in receiver there will be a command implementation. It works as a bridge between receiver and action methods.
Invoker class just forward the request from client to the command object.
Client is responsible to instantiate appropriate command and receiver implementation and then associate them together.
Client is also responsible for instantiating invoker object and associating command object with it and execute the action method.
Command design pattern is easily extendible, we can add new action methods in receivers and create new Command implementations without changing the client code.
The drawback with Command design pattern is that the code gets huge and confusing with high number of action methods and because of so many associations.

# Real World Example.

Resturant is a classic example of Command Pattern.
Customer(Invoker) is not aware of Chef(Receiver) and they communicate via Waiter(Command Manager) by giving Menu Name(Commands) to them.
Customer doesn't need to know how to communicate directly with Chef.


https://sourcemaking.com/design_patterns/command

http://gameprogrammingpatterns.com/command.html

# Code
https://www.tutorialspoint.com/design_pattern/command_pattern.htm
https://dzone.com/articles/design-patterns-command

https://2.bp.blogspot.com/-XO5vlKJvUnk/V4p6hu9a4II/AAAAAAAABF8/2v5jNfytWCckNoLlfxZwMmRgBg9zUz3AQCLcB/s640/command-design-pattern-flow.png
http://gameprogrammingpatterns.com/images/command-buttons-one.png
http://gameprogrammingpatterns.com/images/command-stream.png
http://gameprogrammingpatterns.com/images/command-buttons-two.png
