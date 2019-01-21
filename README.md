## Topics

- Compilation, Interpretation
- Type systems
- Concurrency
- OOP
- Functional programming
- Immutability
- RPC


Source : Wikipedia  




## Variable - Identifier - Value

>In computer programming, a variable or scalar is a **storage location** (identified by a memory address) paired with an associated symbolic name (an identifier), which contains some known or unknown quantity of information referred to as a value.

Think in terms of microprocessors :)

A Variable is a **storage space** (which has a memory address).
**Identifiers** a symbolic name, represents the address of that space
The space can *store* **values** of any type
Throughout the program the space is capable of holding/storing different **value**
Hence the name **variable**

```
var x = 10;

var x; // a space created in memory
x // identifier
10 // value


```

## Declaration vs Definition
Declaration : declaring an **indentifier** with *properties* (public, const, etc)  
Definition  : defining/implementing a declaration with the **value**

A **Variable** is declared and defined


## Statement vs Expressions

Expression definition - Wikipedia
>An expression in a programming language is a combination of one or more *constants, variables, operators, and functions* that the programming language interprets (according to its particular rules of precedence and of association) and **computes** to *produce* ("to **return**", in a stateful environment) another **value**. This process, as for mathematical expressions, is called evaluation.

In simple, expression when computed **returns a value**

Statement definition - Wikipedia
>In computer programming, a statement is a syntactic unit of an **imperative programming language** that expresses some **action to be carried out**.[1] A program written in such a language is formed by a sequence of one or more statements. A statement may have internal components (e.g., expressions).

In simple, statement does actions and won't* return value. **imperative style**
\*in strict sense


Always prefer Expressions over Statements

Expressions are
  - pure
  - won't mutate
  - reusable
  - testable
  - composable
  - easier to express algorithms



## Interface

> In computing, an interface is a shared boundary across which two or more **separate components** of a computer system *exchange information*.


> A software interface may **refer** to a wide range of different types of interface at different "levels"

> in object oriented programs, objects within an application may need to interact via methods

From the above definitions, we can say that,
Interface is a *method/set of methods* that can handle **different types of objects**.  
These different types of objects can **choose an interface** based on the
**purpose** of communication.

> Side Note: Interface in Electrical is the connector - plug(male) and jack(female)
for different electrical systems

### Programming to interface
The idea behind this approach is to *base* programming logic on the interfaces of the objects used, rather than on internal implementation details.

Ref: https://en.wikipedia.org/wiki/Interface_(computing)


In typed languages, Object's **interface** is understood from the **type** it uses
Eg
A Dog object having Animal interface
```
Animal dog = new Dog();
```
This is often used for polymorphism.

> In programming languages and type theory, polymorphism is the *provision* of a **single interface** to entities(objects) of **different types**.

Single Interface for different types.
Here different *types* means different *objects* with different properties

Ref: https://en.wikipedia.org/wiki/Polymorphism_(computer_science)

### Types of Polymorphism
- Ad-hoc polymorphism
- Parametric polymorphism
- Subtyping

> Single Interface --> method that can handle different types --> polymorphic function


#### Ad-hoc polymorphism

> In programming languages, ad hoc polymorphism is a kind of polymorphism in which polymorphic functions can be *applied* to **arguments** of *different types*,
> because a polymorphic function can denote a number of *distinct* and potentially heterogeneous *implementations* *depending on the type of argument(s)* to which it is applied


distinct implementations (as functions) for each types
all their implementations are hidden by providing a single interface.
Interface capable of handling different types

This in some programming language is acheived thru
  - function overloading
  - operator overloading

```


```

#### Parametric Polymorphism
parametric polymorphism, in which polymorphic **functions** are written *without* mention of any *specific type*, and can thus apply a **single abstract implementation** to any number of types in a transparent way.

These functions are also called as **Generics**
Eg: map() function in array.
map() has a *single abstract implementation* that can operate on any object types.
as long as the objects are packed in Array interface

```

```


#### Subtyping polymorphism

> Subtyping should not be confused with the notion of (class or object) inheritance from object-oriented languages;  
>  **subtyping** is a relation between types (**interfaces** in object-oriented parlance) whereas **inheritance** is a relation between **implementations** stemming from a language feature that allows new objects to be created from existing ones.   
> In a number of object-oriented languages, **subtyping** is called **interface inheritance**, with **inheritance** referred to as **implementation inheritance**.
