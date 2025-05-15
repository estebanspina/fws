# Manifesto of the FW Scripting Language

## Introduction

Modern software development —particularly in the web domain— has historically been dominated by imperative and object-oriented paradigms. While these models have provided viable solutions, they also reveal clear limitations in terms of scalability, maintainability, concurrency, and code reasoning.  
In this context, **FWSL (Functional Web Scripting Language)** emerges as a disruptive and necessary proposal: a programming language grounded in the functional paradigm, designed from the ground up for robust, declarative, and highly predictable web development.

## Purpose

The core purpose of FWSL is to establish a new standard for modern web development by naturally and seamlessly promoting the adoption of functional programming principles as a path toward more reliable, testable, and understandable applications, with strict and elegant control over side effects.

## Foundational Principles

FWSL is built upon a set of unwavering principles that form its backbone:

1. **Pure functions as the atomic unit of software:**  
   Every component, transformation, and interaction is modeled as a pure function, with no side effects or reliance on global or external states.

2. **Immutability by default:**  
   All data structures are immutable by design, eliminating entire categories of errors related to mutable state, race conditions, or shared data corruption.

3. **Referential transparency:**  
   In FWSL, any expression can be replaced by its result without altering the program's behavior, ensuring predictable and optimizable semantics.

4. **Declarative function composition:**  
   FWSL promotes building complex solutions by composing simple, reusable, and modular functions, through a clean and expressive syntax.

5. **First-class and higher-order functions with currying as idiomatic practice:**  
   Functions are not only first-class citizens; the language actively encourages the use of higher-order functions, currying, and pointfree styles to achieve maximum expressiveness and abstraction.

6. **Structured and safe side effect management:**  
   FWSL encapsulates all side effects (DOM interactions, IO, errors, asynchronicity) in controlled structures via advanced functional abstractions such as monads, effects, or contexts, thereby preserving the purity of the program's core logic.

## Differentiation

While languages like Elm, PureScript, ClojureScript, and ReasonML explore the space of functional programming applied to the web, FWSL distinguishes itself by:

- **Web-first native design:**  
  FWSL is purposefully designed for the web environment, providing declarative and functional support for interface rendering, state management, event handling, routing, and asynchronous communication.

- **Idiomatic simplicity:**  
  Despite its mathematically rigorous foundation, FWSL offers an accessible, ergonomic syntax focused on a modern developer experience.

- **Extensible controlled effects system:**  
  FWSL provides a flexible and extensible model for effect management, allowing developers to define their own pure abstractions for impure operations.

## Vision

FWSL envisions a future where the **inherent complexity of web development is abstracted away through elegant, predictable, and robust functional models**, freeing developers from the cognitive load of handling mutable states, imperative loops, and error-prone structures.

With FWSL, we aim for web code to be not only correct but also beautiful, clear, and mathematically sound.

## Conclusion

FWSL is not just a language; it is a declaration of principles—a bold commitment to rigor, simplicity, and elegance in web development.  
It is an invitation to rethink how we build the modern web, relying on the proven foundations of functional programming.

## Specification

The complete technical specification, including grammar, type system, semantics, and tooling roadmap, can be found in the [Language Specification](specification.md) file.

## Contribute

## License
