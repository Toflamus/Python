# Design Principles: SOLID

***S:Single Responsibility Principle***  

One class only takes one responsibility

* Easy to maintain  
* Easy to reuse the code

***O: Sopen Closed Principle***  

* Open to extentions
* Colse to modifications

* Can be realised by abstract method and abstract class

***L: liskov Substitution Principle***  

* Locations where a base class reference is used must be able to use objects of the derived class.  

***I: Interface Segregation Principle***  

* A class should not be forced to implement interfaces it does not use.  
* In other words, instead of having a large, monolithic interface that includes methods for various functionalities, it's better to have smaller, more focused interfaces that cater to specific sets of behaviors. Classes should only be required to implement the interfaces that are relevant to their functionality, and they shouldn't be burdened with implementing unnecessary methods.
* The goal of the Interface Segregation Principle is to avoid creating "fat" interfaces that force clients to implement methods they don't need. This enhances the flexibility and maintainability of the code by minimizing dependencies and ensuring that changes to one part of the system do not affect unrelated parts.

***D: Dependency inversion principle***  

* High-level modules should not depend on low-level modules, but both should depend on abstractions (abstract classes or interfaces); and abstractions should not depend on details, but details should depend on abstractions.  

1. High-level modules (which contain the main business logic) should not depend on low-level modules (which implement specific details). Both should depend on abstractions.

2. Abstractions (such as abstract classes or interfaces) should not depend on the details of implementations. Instead, details should depend on abstractions.