# FWSL - Functional Web Scripting Language Specification

## Table of Contents

1. [Introduction](#introduction)
2. [Language Philosophy](#language-philosophy)
3. [Syntax](#syntax)
4. [Semantics](#semantics)
5. [Type System](#type-system)
6. [Core Functional Constructs](#core-functional-constructs)
7. [Standard Library & Web APIs](#standard-library--web-apis)
8. [Tooling & Environment](#tooling--environment)
9. [Examples](#examples)
10. [Minimal Viable Prototype (MVP)](#minimal-viable-prototype-mvp)
11. [Roadmap & Future Work](#roadmap--future-work)

## 1. Introduction

FWSL (Functional Web Scripting Language) is a purely functional, declarative, and modern language designed for web application development. It focuses on immutability, pure functions, declarative composition, and predictable behavior.

## 2. Language Philosophy

- **Purity first:** functions are pure and predictable.
- **Immutability by default:** data is never mutated.
- **Declarative over imperative:** code describes what, not how.
- **Transparent composition:** functions compose naturally.
- **Functional-first for the web.**

## 3. Syntax

### Formal Syntax

```
program        ::= statement*
statement      ::= function_def | expression
function_def   ::= "fun" identifier "(" parameters ")" "=>" expression
parameters     ::= identifier ("," identifier)*
expression     ::= function_call | identifier | literal | composition | "(" expression ")"
function_call  ::= identifier "(" arguments ")"
arguments      ::= expression ("," expression)*
composition    ::= expression "∘" expression
literal        ::= number | string | boolean
identifier     ::= letter (letter | digit)*
number         ::= digit+
string         ::= '"' .*? '"'
boolean        ::= "true" | "false"
```

## 4. Semantics

- Strict evaluation (except composition and currying: lazy).
- Referential transparency: expressions can be replaced with their result.
- Side-effects are isolated and explicit.

### Example

```
fun add(x, y) => x + y
fun double = add(2)
double(5) ; result: 7
```

## 5. Type System

| Type     | Description           |
| -------- | --------------------- |
| Int      | Integer values        |
| String   | Text strings          |
| Bool     | Booleans              |
| List<T>  | Immutable lists       |
| (A -> B) | Functions from A to B |

### Example

```
fun add(x: Int, y: Int): Int => x + y
```

## 6. Core Functional Constructs

- Pure functions
- Currying
- Composition
- Recursion
- Functions as first-class citizens

### Examples

```
fun add(x) => fun(y) => x + y
```
```
fun square(x) => x * x
```
```
fun addThenSquare = square ∘ add(3)
```
```
addThenSquare(4) ; Result: 49
```

##7. Standard Library & Web APIs

### Declarative UI component

```
fun Button(label, onClick) =>
  <button onclick=onClick>{label}</button>
```

### State and controlled side effects

```
fun useState(initial) =>
  (initial, fun(newState) => /* returns new immutable state */)

fun Counter() =>
  let (count, setCount) = useState(0)
  Button("Count: " + count, fun() => setCount(count + 1))
```

## 8. Tooling & Environment

- Compiler from FWSL to optimized JavaScript or WebAssembly.
- Modular system (import, export).
- Testing framework leveraging function purity.
- Integration with browser environments.

