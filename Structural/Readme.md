# Applicability

## Composite
Use the Composite pattern when
- you want to represent part-whole hierarchies of objects.
- you want clients to be able to ignore the difference between compositions of objects and individual objects. Clients will treat all objects in the composite structure uniformly.

```
> Often the component-parent link is used for a Chain of Responsibility.

> Decorator is often used with Composite. When decorators and composites are used together, they will usually have a common parent class. So dcorators will have to support the Component interface with operations like Add, Remove, and GetChild.
```

## Decorator
Use Decorator
- to add responsibilities to individual objects dynamically and transparently, that is, without affecting other objects.
- for responsibilities that can be withdrawn.
- when extension by subclassing is impractical. Sometimes a large number of independent extensions are possible and would produce an explosion of subclasses to support every combination. Or a class definition may be hidden or otherwise unavailable for subclassing.

```
> Composite: A decorator can be viewed as a degenerate composite with only one component. However, a decorator adds additional responsibilities---it isn't intended for object aggregation.

> Strategy: A decorator lets you change the skin of an object; a strategy lets you change the guts. A decorator provides an alternative to subclassing for extending functionality; a strategy provides an alternative to subclassing for varying an algorithm.
```

## Facade
Use the Facade pattern when
- you want to provide a simple interface to a complex subsystem. Subsystems often get more complex as they evolve. Most patterns, when applied, result in more and more classes. This makes the subsystem more reusable and easier to customize, but it also becomes harder to use for clients that don't need to customize it. A facade can provide a simple default view of the subsystem that is good enough for most clients. Only clients needing more customizability will need to look beyond the facade.
- there are many dependencies between clients and the implementation classes of an abstraction. Introduce a facade to decouple the subsystem from clients and other subsystems, thereby promoting subsystem independence and portability.
- you want to layer your subsystems. Use a facade to define an entry point to each subsystem level. If subsystems are dependent, then you can simplify the dependencies between them by making them communicate with each other solely through their facades.

```
> Abstract Factory can be used with Facade to provide an interface fir creating subsystem objects in a subsystem-independant way. Abstract Factory can also be used as an alternative to Facade to hide platform-specific classes.

> Mediator is similar to Facade in that it abstracts functionality of existing classes. However, Mediator's purpose is to abstract arbitrary communication between colleague objects, often centralizing functionality that doesn't belong in any of them. A mediator's colleagues are aware of and communicate with the mediator instead of communicating with each other directly. In contrast, a facade merely abstracts the interface to subsystem objects to make them easier to use; it doesn't define new functionality, and subsystem classes don't know about it.

> Usually only one Facade object is required. Thus Facade objects are often Singletons.
```