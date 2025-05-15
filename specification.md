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

### Formal Syntax (EBNF)

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
