# Design Pattern Practice

## Creational

> Creational design patterns are a category of design patterns that deal with object creation mechanisms, tryinig to create objects in a manner suitable for the situation. They provide flexibility in the way objects are created, and are useful in situations where the type of object to be created is not known in advance, or when you want to delegate the responsibility of object creation to another class.

In plain words
> Creational patterns are focused towards how to instantiate an object or group of related objects.

* [Simple Factory](#simple-factory)
* [Factory Method](#factory-method)
* [Abstract Factory](#abstract-factory)
* [Builder](#builder)
* [Singleton](#singleton)
* [Prototype](#)
---
### Simple Factory
> Generates an instance for client without exposing any instantitation logic to the client.

### Factory Method
> Defines an interface for creating objects, but allows subclasses to decide which class to instantiate.

### Abstract Factory
> A factory of factories; a factory that groups the invidual but related/dependant factories together without specifiying their concrete classes.

#### Participants
- __AbstractFactory__
: declares an interface for operations that create abstract product objects.
- __ConcreteFactory__
: implements the operations to create concrete product objects.
- __AbstractProduct__
: declares an interface for a type of product object.
- __ConcreteProduct__


### Builder
> Separates the construction of a complex object from its representation, allowing the same construction process to create different representation.

### Singleton
> Ensures that only one instance of a class is created, and provides a global point of access to that instance.
---

## Structural
> Structurak design patterns are concerned with object composition and class relationships. They help to create complex structures and provide a way to simplify the structure by identifying the relaionships between the objects.

* [Composite](#composite)
* [Decorator](#decorator)
* [Facade](#facade)
* [Adapter](#)
* [Bridge](#)
* [Flyweight](#)
* [Proxy](#)
---
### Composite
> Composite pattern composes objects into a tree-like structure to represent part-whole hierarhcies. It lets clients treat individual objects and compositions of objects uniformly.

### Decorator
> Decorator pattern lets you dynamically change the behavior of an object at run time by wrapping them in an object of a decorator class, without affecting the behavior of other objects in the same class.

### Facade
> Provides a simplified interface to a complex subsystem, making it easier to use and understand.

---
## Behavioral
> Behavioral design patterns are concerned with the interaction and communication between objects. They help to define common communication patterns between objects, which simplify communication and improve flexibility.

* [Observer](#observer)
* [Mediator](#mediator)
* [Template Method](#template-method)
* [Strategy](#strategy)
* [Chain of Responsibility](#chain-of-responsibility)
* [Command](#)
* [Interpreter](#)
* [Memento](#)
* [State](#)
* [Iterator](#)
* [Visitor](#)

---
### Observer
> Defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.

### Mediator
> Mediator pattern adds a third party object (called mediator) to control the interaction between two objects (called colleagues). It helps reduce the coupling between the classes communicating with each other. Because now they don't need to have the knowledge of each other's implementation.

### Template Method
> Defines the skeleton of an algorithm in a base class and allows subclasses to override specific steps of the algorithm without changing its structure.

### Strategy
> Strategy pattern allows you to switch the algorithm or strategy based upon the situation.

### Chain of Responsibility
> It helps building a chain of objects. Request enters from one end and keeps going from object till it finds the suitable handler.
