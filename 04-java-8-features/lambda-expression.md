## Lambda Expressions (Java 8+)

### What is a Lambda Expression?
A **lambda expression** is a short way to write an **anonymous function** (a function without a name).

### Key Purpose
- Enables **functional programming**
- Reduces **boilerplate code**

---

## Before Java 8 (Anonymous Inner Class)

```java
Runnable runnable = new Runnable() {
    @Override
    public void run() {
        System.out.println("Thread is running");
    }
};
```

---

## After Java 8 (Lambda Expression)

```java
Runnable runnable = () -> System.out.println("Thread is running");
```

---

## Lambda Expression Syntax

### 1. Without Input Parameters
```java
() -> {
    // body
};
```

### 2. With Input Parameters
```java
(parameters) -> {
    // body using parameters
};
```

### Example
```java
(a, b) -> a + b
```

---

## Important Syntax Rules

- Parentheses `()` are optional for a single parameter
- Curly braces `{}` are optional for single-line expressions
- `return` keyword is optional for a single statement
- Data types are optional (type inference)
- Lambda expressions do **not** create a new class

---

## How the Compiler Understands Lambda Expressions

- The **functional interface** determines:
   - Method name
   - Parameter types
   - Return type
- Compiler uses **type inference** to identify return type automatically

---

## Why Do We Use Lambda Expressions?

1. Reduces boilerplate code
2. Code becomes clear and concise
3. Required for Stream API
4. Improves readability
5. Supports functional programming
6. Enables parallel processing
7. Works efficiently with collections

---

## Functional Interface Rule

> A lambda expression can be used **only with a functional interface**

### Functional Interface
An interface with **exactly one abstract method**

Examples:
- `Runnable`
- `Callable`
- `Comparator`
- `Predicate`
- `Function`
- `Consumer`
- `Supplier`

```java
@FunctionalInterface
interface MyInterface {
    void show();
}
```

---

## Limitations

- Cannot be used with interfaces having multiple abstract methods
- Harder to debug if overused
- Not suitable for complex business logic

---

## One-Line Summary

> **Lambda Expression = Concise implementation of a functional interface**
