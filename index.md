## DRY - "DON'T REPEAT YOURSELF"  
The idea here is simple. You should not duplicate the code and reuse it as much as possible.
Do you duplicate the same line 5 times? Write a loop. 
Do you duplicate the same instructions with different parameters? Write a function. 
Do you duplicate a set of functions? Write a class. 
Do you duplicate the same class for different types? Write generic.
## KISS - "KEEP IT SIMPLE, STUPID"  
It anticipates that most stuff works best if they are kept simple rather than made complicated.
## YAGNI - "YOU AREN'T GOING TO NEED IT"  
Meaning, you should not add a logic that is not used right now, but for the future.
Why invest time in functionality that's not needed?
## Tell Don't Ask
The idea here is that you should tell an object to perform some logic, rather than asking its state to do an action yourself.
## Divide and Conquer
The core idea is as old as time: split the problem into smaller parts, solve each part, and combine the results.
## CQS - "Command-query separation"
It says the function should either be a command that executes an action or a query that returns data, but not both.
## SOLID
### S (Single responsibility principle)
There should never be more than one reason for a class to change.
In other words, every class should have a single responsibility.
What do you define by responsibility? There are obvious cases when your single class doing math calculations, payments, data storage, email notifications, and so on. Surely it has not been decomposed properly. 
But there are also not-so-obvious ones. The issue here, it is not clear where you define those boundaries and draw the line. This principle does not tell anything.
### O (Open/Closed principle)
Software entities should be open for extension, but closed for modification. 
That is, such an entity can allow its behaviour to be extended without modifying its source code.
Or, design your code in a way, that adding a new feature means creating new classes and not editing existing code.
### L (Liskov substitution principle)
Functions that use pointers or references to base classes must be able to use objects of derived classes without knowing it.
In human words, you should be able to use subclass everywhere where parent class is used.
### I (Interface segregation principle)
Clients should not be forced to depend upon interfaces that they do not use.
Or, don't put all methods in a single interface.
Just have separate interfaces, and implement them based on your needs.
### D (Dependency inversion principle)
- Depend upon abstractions, not implementation.
- Developers usually will say something like:
High-level modules should not depend on low-level modules. Both should depend on abstractions
Abstractions should not depend on details. Details should depend on abstractions.  
In simpler terms, you have two types of dependencies:  
- code dependency, when one class (or module) depends on another
- execution flow, when one class (or module) calls another
