# Chapter 3 – Principles of Object-Oriented Design

## Sections

1. Principle 1: Single Responsibility
2. Principle 2: Separation of Concerns
3. Principle 3: DRY (Don’t Repeat Yourself)
4. Principle 4: Open for Extension, Closed for Modification
5. Principle 5: Separation of Interfaces from Implementations
6. Principle 6: Dependency Inversion

   * Inversion of Control
7. Principle 7: Make It Testable

---

## Summary

This chapter introduces the core **design principles** that guide effective object-oriented software development. Rather than focusing on language features, it emphasizes **how to structure software** so that it remains understandable, adaptable, and resilient to change. Each principle addresses a specific aspect of managing complexity, reducing coupling, and improving maintainability. Together, these principles form a practical framework for making design decisions and evaluating the quality of object-oriented systems.

---

## Key Concepts

### 1. Single Responsibility Principle

* Each class or module should have **one clear responsibility** and **one reason to change**.
* Encourages small, focused abstractions with well-defined roles.
* Reduces the risk that changes in one area cause unintended side effects elsewhere.
* Improves readability, maintainability, and testability.

---

### 2. Separation of Concerns

* Different aspects of a system should be **isolated** from one another.
* Each concern (e.g., business logic, persistence, presentation) should be handled independently.
* Limits complexity by preventing unrelated logic from being interwoven.
* Forms the basis for layered architectures and modular system design.

---

### 3. DRY (Don’t Repeat Yourself)

* Knowledge and logic should be **expressed in a single place** within the system.
* Duplication increases maintenance effort and risk of inconsistent behavior.
* DRY applies to:

  * Code,
  * Business rules,
  * Configuration and documentation.
* Promotes reuse through abstraction, not copy-and-paste.

---

### 4. Open for Extension, Closed for Modification

* Software entities should be **extendable without altering existing code**.
* New behavior is added through:

  * Polymorphism,
  * Composition,
  * New implementations of existing interfaces.
* Minimizes regression risk and preserves system stability.
* Encourages anticipation of change without premature generalization.

---

### 5. Separation of Interfaces from Implementations

* Clients depend on **what a component does**, not on **how it does it**.
* Interfaces define contracts; implementations provide concrete behavior.
* Enables independent evolution of implementations.
* Supports substitutability, mocking, and flexible system composition.

---

### 6. Dependency Inversion

* High-level modules should not depend on low-level modules; both should depend on **abstractions**.
* Details depend on policies, not the other way around.
* Reduces coupling and increases flexibility in system architecture.
* Often implemented using interfaces or abstract base classes.

#### Inversion of Control

* The control flow of object creation and collaboration is **delegated to a framework or container**.
* Objects do not instantiate their dependencies directly.
* Enables configuration-driven composition and late binding of implementations.
* Commonly realized via dependency injection mechanisms.

---

### 7. Make It Testable

* Design should facilitate **automated testing** at unit and integration levels.
* Testable code is typically:

  * Loosely coupled,
  * Deterministic,
  * Based on clear interfaces.
* Dependencies should be replaceable with mocks or stubs.
* Testability is a strong indicator of overall design quality.

---

## Notes & Reflections

* These principles are not rigid rules but **guidelines** that inform design trade-offs.
* Applying them consistently leads to systems that are easier to evolve and reason about.
* Testability acts as a unifying theme: designs that follow these principles tend to be naturally testable.
