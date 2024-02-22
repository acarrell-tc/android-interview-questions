Object-Oriented Programming Interview Questions
===============================================

* [1. Can you explain the four main principles of Object-Oriented Programming (OOP)?](#1-can-you-explain-the-four-main-principles-of-object-oriented-programming-oop)
* [2. How would you differentiate between a class and an object?](#2-how-would-you-differentiate-between-a-class-and-an-object)
* [3. Can you explain the Law of Demeter (LoD) and its significance in OOP?](#3-can-you-explain-the-law-of-demeter-lod-and-its-significance-in-oop)
* [4. How does encapsulation help in the maintenance and organization of code in OOP?](#4-how-does-encapsulation-help-in-the-maintenance-and-organization-of-code-in-oop)
* [5. Can you explain polymorphism with a practical example?](#5-can-you-explain-polymorphism-with-a-practical-example)
* [6. How is data abstraction implemented in OOP?](#6-how-is-data-abstraction-implemented-in-oop)
* [7. Can you define a virtual function and its use in OOP?](#7-can-you-define-a-virtual-function-and-its-use-in-oop)
* [8. How would you differentiate between overloading and overriding in OOP?](#8-how-would-you-differentiate-between-overloading-and-overriding-in-oop)
* [9. Explain how inheritance improves code reusability in OOP.](#9-explain-how-inheritance-improves-code-reusability-in-oop)
* [10. Can you discuss the use of interfaces in OOP languages like Java or C#?](#10-can-you-discuss-the-use-of-interfaces-in-oop-languages-like-java-or-c)
* [11. What are the different types of inheritance in OOP? Explain with examples.](#11-what-are-the-different-types-of-inheritance-in-oop-explain-with-examples)
* [12. Define composition. How does it differ from inheritance?](#12-define-composition-how-does-it-differ-from-inheritance)
* [13. Discuss the problems that can occur from multiple inheritances and how you would avoid them.](#13-discuss-the-problems-that-can-occur-from-multiple-inheritances-and-how-you-would-avoid-them)
* [14. How do you achieve loose coupling in OOP design?](#14-how-do-you-achieve-loose-coupling-in-oop-design)
* [15. Describe the concept of “method hiding” in OOP.](#15-describe-the-concept-of-method-hiding-in-oop)
* [16. Can you explain the role of constructors and destructors in OOP?](#16-can-you-explain-the-role-of-constructors-and-destructors-in-oop)
* [17. How is exception handling performed in OOP?](#17-how-is-exception-handling-performed-in-oop)
* [18. What is the Singleton design pattern? Give a practical example of where it would be useful.](#18-what-is-the-singleton-design-pattern-give-a-practical-example-of-where-it-would-be-useful)
* [19. Can you explain the concept of an abstract class in OOP?](#19-can-you-explain-the-concept-of-an-abstract-class-in-oop)
* [20. How do you ensure thread safety in an object-oriented program?](#20-how-do-you-ensure-thread-safety-in-an-object-oriented-program)
* [21. What are the SOLID principles of OOP? Can you give examples of each?](#21-what-are-the-solid-principles-of-oop-can-you-give-examples-of-each)
* [22. Explain the concept of dependency injection and how it improves code modularity in OOP.](#22-explain-the-concept-of-dependency-injection-and-how-it-improves-code-modularity-in-oop)
* [23. What are the different types of class relationships in OOP?](#23-what-are-the-different-types-of-class-relationships-in-oop)
* [24. Can you explain the factory design pattern and its use cases?](#24-can-you-explain-the-factory-design-pattern-and-its-use-cases)
* [25. How would you implement data hiding in OOP and why is it important?](#25-how-would-you-implement-data-hiding-in-oop-and-why-is-it-important)

### 1. Can you explain the four main principles of Object-Oriented Programming (OOP)?

Object-Oriented Programming (OOP) is based on four main principles: encapsulation, inheritance, polymorphism, and
abstraction. Encapsulation refers to the bundling of data with methods that operate on that data. It restricts direct
access to some components, ensuring integrity by hiding internal states and values inside a class. Inheritance allows
classes to inherit features of other classes, promoting code reusability and logical structure. Polymorphism enables one
interface to be used for a general class of actions; it provides flexibility while implementing functions with the same
name but different functionalities. Abstraction simplifies complex systems by modeling them in a manner that focuses on
relevant details; it hides unnecessary complexity from the user. These principles are fundamental to OOP, providing a
clear modular structure for programs which makes it good for defining abstract datatypes where implementation details
are hidden.

### 2. How would you differentiate between a class and an object?

A class in Object-Oriented Programming (OOP) is a blueprint or template that defines the variables and methods common to
all objects of a certain kind. It encapsulates data for the object. An object, on the other hand, is an instance of a
class. It’s created from the class blueprint and can have unique values. While multiple objects can be instantiated from
one class, each has its own memory space and set of properties. The class represents the abstract concept while the
object embodies the concrete instance of that concept.

### 3. Can you explain the Law of Demeter (LoD) and its significance in OOP?

The Law of Demeter (LoD) is a design guideline in OOP, promoting loose coupling among software components. It states
that an object should only communicate with its immediate neighbors and not with objects indirectly associated with it.
This law reduces dependencies between classes or objects, making the system more modular and easier to maintain.

In essence, LoD discourages deep navigation into object structures as it leads to high coupling and fragile code. If an
object needs data from a distant relation, it’s better to have the data passed through intermediate objects.

For instance, if class A uses class B which uses class C, then according to LoD, A shouldn’t directly call methods on C
but instead ask B to perform operations involving C. This way, changes in C won’t affect A, enhancing modularity and
robustness.

However, applying LoD strictly can lead to bloated interfaces where classes have many trivial methods just to comply
with the law. Therefore, it’s important to strike a balance based on specific project requirements.

### 4. How does encapsulation help in the maintenance and organization of code in OOP?

Encapsulation, a fundamental principle of OOP, enhances code maintenance and organization by bundling data with the
methods that manipulate it. It restricts direct access to an object’s data, ensuring integrity by preventing accidental
or unauthorized modifications. Encapsulation also promotes modularity; objects can be understood independently,
simplifying debugging and testing. By hiding internal workings, changes in one part of the system don’t necessitate
changes elsewhere, reducing dependencies and increasing flexibility.

### 5. Can you explain polymorphism with a practical example?

Polymorphism, a key principle in OOP, allows objects of different classes to be treated as objects of a common
superclass. It enhances flexibility and maintainability by allowing one interface with many implementations.

Consider an example: a superclass ‘Animal’ with a method ‘sound()’. Subclasses ‘Dog’, ‘Cat’, and ‘Bird’ each override
this method to return their unique sounds. In the main program, we create an array of Animal references, where each
element points to an instance of Dog, Cat, or Bird. When we iterate over this array and call ‘sound()’ for each object,
the appropriate subclass’s sound is produced. This is polymorphism – the ability to present the same interface for
differing underlying forms (data types).

### 6. How is data abstraction implemented in OOP?

Data abstraction in OOP is implemented through encapsulation and interfaces. Encapsulation hides the internal states of
an object by only allowing access to it through methods, ensuring data integrity. Interfaces provide a way for objects
to interact with each other without revealing their implementation details. This allows changes in one part of a system
without affecting others.

### 7. Can you define a virtual function and its use in OOP?

A virtual function is a member function in the base class that we expect to redefine in derived classes. It’s declared
using the keyword ‘virtual’ and primarily used for achieving runtime polymorphism. When a class contains a virtual
function, it maintains a vtable (virtual table) containing addresses of its virtual functions. This allows dynamic
linkage to occur when a virtual function is called on an object pointer or reference, directing us to the correct
function even if the exact type of the object isn’t known at compile time. Thus, virtual functions enable us to design
more flexible and reusable components by allowing subclasses to provide their specific implementation without changing
interface code.

### 8. How would you differentiate between overloading and overriding in OOP?

Overloading and overriding are both techniques in OOP, but they serve different purposes. Overloading occurs when two or
more methods in the same class have the same name but different parameters. It’s a way to perform one action in
different ways. For example:

```java
public int add(int a, int b) {
    return a + b;
}

public double add(double a, double b) {
    return a + b;
}
```

On the other hand, overriding is used for runtime polymorphism. A subclass has the same method as declared in the parent
class. Here, the method in the child class will be executed not the one in the parent class. Example:

```java
class Parent {
    void show() {
        System.out.println("Parent's show");
    }
}

class Child extends Parent {
    void show() {
        System.out.println("Child's show");
    }
}
```

### 9. Explain how inheritance improves code reusability in OOP.

Inheritance in OOP enhances code reusability by allowing new classes to adopt properties and methods from existing ones,
reducing redundancy. A base class (parent) shares its attributes with derived classes (children), which can also have
unique features. This hierarchy allows for modification of shared characteristics in one location, the parent class,
affecting all inheriting classes, promoting DRY (Don’t Repeat Yourself) principle. It simplifies debugging and updating
as changes need only be made once at a common point. However, it’s crucial to ensure logical relationships between
classes to avoid inappropriate inheritance that could complicate rather than simplify the system.

### 10. Can you discuss the use of interfaces in OOP languages like Java or C#?

Interfaces in OOP languages like Java or C# are used to define a contract for classes, without implementing any
behavior. They declare methods and variables that a class must implement if it uses the interface. This promotes code
reusability and modularity, as different classes can use the same interface but provide different implementations.
Interfaces also support polymorphism; an object of a class implementing an interface can be treated as an object of the
interface type. In addition, they enable safe, flexible functionality sharing between unrelated classes. For instance,
Comparable and Serializable interfaces in Java allow objects of diverse classes to be sorted or serialized respectively.

### 11. What are the different types of inheritance in OOP? Explain with examples.

Inheritance in OOP is a mechanism where one class acquires properties of another. There are four types: single,
multiple, multilevel, and hierarchical.

Single inheritance allows a derived class to inherit from only one base class. For example, if we have a base class
‘Animal’ and a derived class ‘Dog’, the ‘Dog’ class can inherit characteristics like ‘breathing’ or ‘eating’ from
‘Animal’.

Multiple inheritance permits a class to inherit from more than one base class. If we have two base classes ‘Flying’ and
‘Swimming’, and a derived class ‘Duck’, ‘Duck’ can inherit abilities from both ‘Flying’ and ‘Swimming’.

Multilevel inheritance involves a chain of classes inheriting from each other. For instance, if we have three classes
‘Mammal’, ‘Primate’, and ‘Human’, ‘Human’ inherits from ‘Primate’, which inherits from ‘Mammal’.

Hierarchical inheritance allows one base class to be inherited by many derived classes. If ‘Vehicle’ is our base class,
it could be inherited by several derived classes such as ‘Car’, ‘Bike’, and ‘Bus’.

### 12. Define composition. How does it differ from inheritance?

Composition is a design technique in object-oriented programming where a class is constructed by using references to
other classes. It allows for code reuse, flexibility and maintainability. In composition, if the parent class ceases to
exist, so does its child class, demonstrating a “has-a” relationship.

In contrast, inheritance involves creating new classes from existing ones, forming a “is-a” relationship. The derived
class inherits properties and behavior of the base class, but can also override or extend them. If the parent class is
deleted, the child class still exists independently.

While both techniques promote code reuse, they differ in their degree of coupling and dependency. Composition provides
loose coupling, making components more independent and interchangeable. Inheritance creates tight coupling due to
hierarchical relationships, which may lead to inflexibility when changes are needed.

### 13. Discuss the problems that can occur from multiple inheritances and how you would avoid them.

Multiple inheritance can lead to several issues in OOP. The most common problem is the Diamond Problem, where a class
inherits from two classes that have a common base class. This leads to ambiguity as it’s unclear which parent class
method should be used. Another issue is increased complexity and potential redundancy, making code harder to maintain.

To avoid these problems, we can use interfaces or abstract classes instead of multiple inheritances. These provide a
structure for subclasses without causing conflicts. Composition over inheritance principle can also be applied, where
objects are designed to contain instances of other objects rather than inheriting properties from a parent class.

### 14. How do you achieve loose coupling in OOP design?

Loose coupling in OOP design is achieved through several strategies. The first strategy involves the use of interfaces
and abstract classes, which allow objects to interact without knowing each other’s concrete types. This reduces
dependency between classes.

The second strategy is encapsulation, where data and methods are bundled into single units or classes. By hiding
internal states and requiring interaction via methods, we limit external dependencies.

Thirdly, using composition over inheritance can also lead to loose coupling. Instead of inheriting properties from a
parent class, an object is composed of other objects, reducing the risk of tight coupling that comes with deep
inheritance hierarchies.

Dependency injection is another method for achieving loose coupling. It allows us to pass dependencies into an object
externally rather than having the object create them itself. This makes our code more flexible and easier to test.

Lastly, the principle of least knowledge (Law of Demeter) advises an object to only communicate with its immediate
neighbors and not with objects indirectly related to it. This prevents unnecessary dependencies and promotes loose
coupling.

### 15. Describe the concept of “method hiding” in OOP.

Method hiding in OOP is a concept related to inheritance. When a subclass has a method with the same name as a
superclass, it hides the superclass’s method. This occurs even if the methods have different parameters. The hidden
method of the superclass can still be accessed using an object reference variable of the superclass type. However, when
the subclass’s method is invoked, it will execute instead of the superclass’s method. This is not polymorphism or
overriding; it’s simply that the subclass’s method takes precedence over the superclass’s method.

### 16. Can you explain the role of constructors and destructors in OOP?

Constructors and destructors are special member functions in OOP. A constructor is invoked when an object of a class is
created, initializing the object’s data members and allocating memory if necessary. It can be overloaded to support
different initialization strategies.

A destructor, on the other hand, is called when an object goes out of scope or is explicitly deleted. Its main role is
to deallocate memory that was previously allocated by the constructor, preventing memory leaks. This ensures efficient
use of resources.

In essence, constructors equip objects with initial states while destructors clean up any resources the object used
during its lifetime, maintaining system stability and performance.

### 17. How is exception handling performed in OOP?

Exception handling in OOP is performed using a system of try, catch, and finally blocks. When an exception occurs within
the ‘try’ block, execution stops and control shifts to the first ‘catch’ block that matches the type of exception
thrown. If no match is found, it’s considered unhandled and program terminates. The ‘finally’ block executes regardless
of whether an exception was thrown or caught. This ensures cleanup code always runs. In languages like Java, exceptions
are objects derived from Throwable class. Two main types exist: checked (compile-time) and unchecked (runtime). Checked
exceptions must be declared in method signature or handled within method body.

### 18. What is the Singleton design pattern? Give a practical example of where it would be useful.

The Singleton design pattern is a creational design pattern that ensures only one instance of a class exists and
provides a global point of access to it. It’s useful when exactly one object is needed to coordinate actions across the
system.

A practical example would be a logging class. A single log file should exist in an application, which handles all
logging operations. Creating multiple instances could lead to overwriting or missing logs. The Singleton pattern can
ensure that all logs are directed to a single file from different parts of an application.

Here’s a simple Python implementation:

```
class Logger:
    _instance = None
    @staticmethod 
    def getInstance():
        if Logger._instance == None:
            Logger()
        return Logger._instance
    def __init__(self):
        if Logger._instance != None:
            raise Exception("This class is a singleton!")
        else:
            Logger._instance = self
```

### 19. Can you explain the concept of an abstract class in OOP?

An abstract class in OOP is a blueprint for other classes, providing a common interface. It’s designed to be extended by
subclasses and cannot be instantiated directly. Abstract classes contain at least one abstract method – a method
declared but not implemented within the abstract class itself. The implementation of these methods is provided by any
class that inherits from the abstract class. This allows for code reusability and polymorphism as different subclasses
can provide different implementations of the same abstract method while still being treated uniformly by code that
operates on the superclass level.

### 20. How do you ensure thread safety in an object-oriented program?

Thread safety in an object-oriented program can be ensured through various strategies. One common approach is
synchronization, where shared resources are accessed by only one thread at a time using locks or mutexes. This prevents
race conditions and ensures data consistency.

Another strategy is immutability, where objects cannot be modified after creation. Immutable objects are inherently
thread-safe as they do not have variable state.

A third method is ThreadLocal storage, which provides each thread its own instance of a variable, eliminating conflicts
between threads.

Lastly, atomic operations can also ensure thread safety. These operations complete in a single step without the
possibility of interference from other threads.

### 21. What are the SOLID principles of OOP? Can you give examples of each?

SOLID principles are fundamental concepts in OOP.

1. Single Responsibility Principle (SRP): A class should have only one reason to change. For instance, a ‘Customer’
   class should handle customer-related tasks but not order processing.

2. Open-Closed Principle (OCP): Software entities should be open for extension but closed for modification. An example
   is adding new features via inheritance rather than modifying existing code.

3. Liskov Substitution Principle (LSP): Subtypes must be substitutable for their base types. If ‘Bird’ is a class and
   ‘Duck’ is a subclass, wherever Bird is used, Duck can also be used without causing issues.

4. Interface Segregation Principle (ISP): Clients shouldn’t be forced to depend on interfaces they don’t use. For
   example, if a class implements an interface with methods it doesn’t need, it violates ISP.

5. Dependency Inversion Principle (DIP): High-level modules shouldn’t depend on low-level ones; both should depend on
   abstractions. This could mean using interfaces or abstract classes to decouple dependencies between classes.

### 22. Explain the concept of dependency injection and how it improves code modularity in OOP.

Dependency Injection (DI) is a design pattern in OOP that decouples objects and their dependencies. Instead of an object
creating its own dependencies, they are supplied externally, typically through the constructor or setter methods. This
allows for greater flexibility as dependencies can be swapped out easily without modifying the dependent class.

In terms of code modularity, DI promotes high cohesion and low coupling. High cohesion means each module has a single,
well-defined task. Low coupling implies minimal dependency between modules. By injecting dependencies, we ensure that
each class focuses on its core responsibility, enhancing cohesion.

Moreover, it reduces the interdependency between classes, fostering loose coupling. If a class changes, there’s less
likelihood of affecting others since dependencies are not hard-coded but injected.

Furthermore, DI facilitates unit testing by allowing mock objects to replace real ones, isolating the behavior of the
class under test. Thus, DI significantly improves code modularity, making it more maintainable, flexible, and testable.

### 23. What are the different types of class relationships in OOP?

In Object-Oriented Programming, there are three primary types of class relationships: association, aggregation, and
inheritance.

Association is a broad term that encompasses any relationship between classes. It can be one-to-one, one-to-many, or
many-to-many. For instance, an employee works for a company; this is a one-to-many association.

Aggregation represents a “has-a” relationship where one object owns or contains another but both can exist
independently. An example would be a car and its engine; the car has an engine, but both can exist separately.

Inheritance depicts an “is-a” relationship, signifying that one class is a subtype of another. The subclass inherits
attributes and methods from the superclass, promoting code reusability. A dog is an animal, so in OOP, the Dog class
could inherit from the Animal class.

### 24. Can you explain the factory design pattern and its use cases?

The factory design pattern is a creational pattern in OOP that provides an interface for creating objects, but allows
subclasses to alter the type of objects created. It promotes loose coupling by eliminating the need to bind
application-specific classes into code. The client code interacts with this interface to create new objects, making it
easier to manage and manipulate these instances.

Use cases include:

1. When a class can’t anticipate the type of objects it needs to create.
2. When a class wants its subclasses to specify the objects it creates.
3. To encapsulate complex creation logic or when there’s a significant genericity involved in object creation.

For instance, consider a UI library where buttons may vary (WindowsButton, HTMLButton). A button factory determines the
type of button to create based on input parameters. This abstracts away complexities from the client code, enhancing
maintainability and scalability.

### 25. How would you implement data hiding in OOP and why is it important?

Data hiding in OOP is implemented through encapsulation, which involves making the data members private and providing
public getter and setter methods. This ensures that the internal state of an object can only be changed via these
methods, preventing direct access to its fields.

This concept is crucial for several reasons. Firstly, it enhances security by restricting unauthorized access to
sensitive data. Secondly, it promotes modularity as each object manages its own data independently. Thirdly, it allows
for greater control over what values can be assigned to the data members, ensuring data integrity.

For instance, consider a class ‘BankAccount’ with a private field ‘balance’. The balance cannot be directly accessed or
modified from outside the class. Instead, we provide public methods like ‘deposit’ and ‘withdraw’, which include
necessary checks and validations before modifying the balance.

```java
public class BankAccount {
    private double balance;

    public void deposit(double amount) {
        if (amount > 0)
            this.balance += amount;
    }

    public void withdraw(double amount) {
        if (amount <= this.balance)
            this.balance -= amount;
    }
}
```

Source: https://interviewprep.org/object-oriented-programming-oop-interview-questions/