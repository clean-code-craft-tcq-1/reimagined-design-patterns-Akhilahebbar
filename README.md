# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

# ADAPTER DESIGN PATTERN
It is of structural type design pattern. Adapter design pattern can be used when two incompatible interfaces need to communicate with each other.  The adapter act as a translator or converter between different adaptees .It will make the client unaware of the complexity of conversion. It acts as a wrapper for multiple interfaces to hide the complexity from the client.
Example: Two members are added to a project. But they both don't understand others language.(one knows only Korean and other knows only German).In order to make the project success both need to communicate.
In that situation we can introduce one more member who knows both (Adapter).So that he can translate by communicate with the other two members.
> Advantages:
- It acts as a wrapper for multiple interfaces to hide the complexity from the client.
- This helps to reuse the existing code.
- Different incompatible interfaces can communicate.
- Adapter hides the things after they designed.
- Can provide the expected form of data to client even though it is not there in existing system.(no need to modify existing code)
> Disadvantages:
- The two objects must be similar or must have same features
- All communication happen though adapter.

# BRIDGE DESIGN PATTERN
It is of structural type design pattern. As the name suggests ,bridge design pattern is used to connect two units of code. In some situation we need to separate units of code so that to maximize the code reusability but we need those to be connected to work as a overall .In that situation, Bridge design pattern helps. Major steps of design pattern is to break the entire thing to abstraction and implementation.

Example: USB cable charger. In this example USB cable will act as bridge. Using cable we can charge phone and we can connect phone to laptop also. If cable fails nothing will work. But If independent unit(phone/laptop/charger) fails ,then the other one will work.
> Advantages:
- Increases code reusability
- Reduces code duplication
- Maximizes the code maintainability
- Minimizes code modification after design
- Increase the productivity as it saves both development and testing efforts 
- follows Single Responsibility principle

> Disadvantages:
- if two processes/unit of code are separable then only we can use this design pattern.
- The separated functions should be able to work independently
- This must be planned before development, if we plan in between then it requires more effort.
- If common code/function fails the everything fails.
- Changes in common function is difficult as this code can be used by multiple functions

# BUILDER DESIGN PATTERN
This is the simplest of all design pattern. As the name suggests ,it goes as a step by step process. This pattern separates construction of complex object from the representation of the final output.
Example: Preparing burger .In this, first we place bread ,on top we place cheese ,then salad ,then tikki, then we place cheese, then bread. Everything will be followed one after the other. Ad this keeps the preparation of bread away from making burger.

> Advantages:
- Allows user to vary a output's internal representation.
- Encapsulates code for construction and representation.
- Full control on construction steps.

> Disadvantages:
- Data members of class aren’t guaranteed to be initialized.
- Dependency injection may be less supported.

