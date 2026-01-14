# Assignment 2 – Vehicle Management System

## Project Overview
This project was created as part of Assignment 2 for the Object-Oriented Programming course.  
The goal of the project is to demonstrate core OOP concepts such as inheritance, abstraction,
composition, and method overriding using a simple Vehicle Management System.

The system includes different types of vehicles that share common behavior through an
abstract superclass while implementing their own specific functionality.

---

## OOP Concepts Used

### Abstraction
An abstract class `Vehicle` is used to define common fields and abstract methods
such as `startEngine()` and `stopEngine()`.

### Inheritance
The classes `Car`, `Motorcycle`, and `Truck` extend the `Vehicle` class and inherit
its properties and methods.

### Method Overriding
Each subclass provides its own implementation of the `startEngine()` and
`stopEngine()` methods.

### Composition and Aggregation
Each `Vehicle` object has a `Driver` object (composition), and one `Driver`
can be associated with multiple `Vehicle` objects (aggregation).

---

## Class Hierarchy

- Vehicle (abstract)
  - Car
  - Motorcycle
  - Truck

The `Vehicle` class uses protected fields to allow subclasses to access common
data while maintaining encapsulation.

---

## How to Compile and Run

From the `src` directory, run the following commands:

```bash
javac *.java
java Main
Program Output
The program demonstrates:
Starting and stopping engines for different vehicle types
Displaying vehicle information
Displaying driver information
Polymorphic behavior using an array of Vehicle objects
Reflection
Inheritance simplified the system design by allowing common attributes and
methods to be shared across all vehicle types. Method overriding made it possible
to customize behavior for each specific vehicle while keeping a consistent
interface. One challenge was correctly organizing files and understanding how
protected fields work across subclasses.
