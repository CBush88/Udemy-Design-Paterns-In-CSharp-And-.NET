# Udemy-Design-Paterns-In-CSharp-And-.NET

Creational Design Patterns

Builder
  Separate component for when object construction gets too complicated
  Can create mutually cooperating sub-builders
  Often has a fluent interface

Factories
  Factory method more expressive than constructor
  Different name than class, different argument names
  Factory can be outside class or inner class; inner class has the benefit of accessing private members

Prototype
  Creation of object from existing object
  Requires either explicit deep copy or copy through serialization

Singleton
  When you need to ensure just a single instance exists
  Made thread-safe and lazy with Lazy<T>
  Consider extracting interface or using dependency injection



Structural Design Patterns

Adapter
  Converts the interface you get to the interface you need

Bridge
  Decouples abstraction from implementation

Composite
  Allows clients to treat individual objects and compositions of objects uniformly

Decorator
  Attach responsibilities to objects
  "Inherit from sealed classes; emulate multiple inheritance

Facade
  Provide a single unified interface over a set of classes/systems

Flyweight
  Efficiently support very large numbers of similar objects

Proxy
  Provide a surrogate object that forwards calls to the real object while performing additional functions
  Eg. Access control, communication, logging, etc.
  Dynamic proxy creates a proxy dynamically, without the necessity of replicating the target object API



Behavioral Design Patterns

Chain of Responsibility
  Allow components to process information/events in a chain
  Each element in the chain refers to the next element; or
  Make a list and go through it

Command
  Encapsulate a request into a separate object
  Good for audit, replay, undo/redo
  Part of Command Query Separation / Command Query Responsibility Separation (Query is also, effectively, a command)

Interpreter
  Transform textual input into object-oriented structures
  Used by interpreters, compilers, static analysis tools, etc.
  Compiler Theory is a separate branch of Computer Science

Iterator
  Provides an interface for accessing elements of an aggregate object
  IEnumerable<T> should be used in 99% of cases

Mediator
  Provides mediation between two objects
  Eg. message passing, chat room

Memento
  Yields tokens representing system states
  Tokens do not allow direct manipulation, but can be used in appropriate APIs

Observer
  Built into C# with the event keyword
  Additional support provided for properties, collections and observable streams

State
  We model systems by having one of a possible set of states and transition between these states
  Such a system is called a state machine
  Special frameworks exist to orchestrate state machines

Strategy and Template Method
  Both patterns define an algorithm blueprint/placeholder
  Strategy uses Composition, Template Method uses inheritance

Visitor
  Adding functionality to existing classes through double dispatch
  Dynamic visitor possible, but with performance cost

