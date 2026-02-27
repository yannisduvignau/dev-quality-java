# 🏛️ dev-quality-java

> **Development Quality** — A university course exploring classic **Gang of Four (GoF) Design Patterns** implemented in Java, alongside object-oriented relationship modeling.

---

## 📋 Description

**dev-quality-java** is an academic repository dedicated to software design quality in Java. It covers five foundational **GoF design patterns** — structural, behavioral, and creational — each implemented in a self-contained module with practical examples.

The repository also includes an exercise on **symmetric 1-to-N relationships**, a key concept in object-oriented modeling that ensures bidirectional consistency between associated objects.

---

## 🗂️ Project Structure

```
dev-quality-java/
├── DESIGN_PATTERN_Adaptateur/       # Adapter pattern (Structural)
├── DESIGN_PATTERN_Composite/        # Composite pattern (Structural)
├── DESIGN_PATTERN_Observateur/      # Observer pattern (Behavioral)
├── DESIGN_PATTERN_Strategie/        # Strategy pattern (Behavioral)
├── DESIGN_PATTER_Mediateur/         # Mediator pattern (Behavioral)
└── RelationSymetrique1xN/           # Symmetric 1-to-N OO relationship
```

---

## 🎨 Design Patterns Overview

### 🔌 Adapter — `DESIGN_PATTERN_Adaptateur`
> **Category:** Structural

The **Adapter** pattern converts the interface of a class into another interface that clients expect. It acts as a bridge between incompatible interfaces, enabling classes to work together that otherwise couldn't.

**Use case:** Wrapping a legacy component or third-party library to fit into a new system without modifying the original code.

**Key participants:** `Target`, `Adapter`, `Adaptee`, `Client`

---

### 🌲 Composite — `DESIGN_PATTERN_Composite`
> **Category:** Structural

The **Composite** pattern composes objects into tree structures to represent part-whole hierarchies. It lets clients treat individual objects and compositions of objects uniformly.

**Use case:** Representing file systems (files and directories), UI component trees, or organizational charts.

**Key participants:** `Component`, `Leaf`, `Composite`, `Client`

---

### 👁️ Observer — `DESIGN_PATTERN_Observateur`
> **Category:** Behavioral

The **Observer** pattern defines a one-to-many dependency between objects so that when one object (the subject) changes state, all its dependents (observers) are notified and updated automatically.

**Use case:** Event systems, MVC architectures, real-time dashboards, or notification systems.

**Key participants:** `Subject`, `Observer`, `ConcreteSubject`, `ConcreteObserver`

---

### ♟️ Strategy — `DESIGN_PATTERN_Strategie`
> **Category:** Behavioral

The **Strategy** pattern defines a family of algorithms, encapsulates each one, and makes them interchangeable. The strategy lets the algorithm vary independently from the clients that use it.

**Use case:** Sorting strategies, payment processing methods, compression algorithms, or routing logic.

**Key participants:** `Context`, `Strategy`, `ConcreteStrategyA`, `ConcreteStrategyB`

---

### 📡 Mediator — `DESIGN_PATTER_Mediateur`
> **Category:** Behavioral

The **Mediator** pattern defines an object that encapsulates how a set of objects interact. It promotes loose coupling by keeping objects from referring to each other explicitly and allows you to vary their interaction independently.

**Use case:** Chat room systems, air traffic control, complex UI form interactions, or event bus architectures.

**Key participants:** `Mediator`, `ConcreteMediator`, `Colleague`, `ConcreteColleague`

---

### 🔗 Symmetric 1-to-N Relationship — `RelationSymetrique1xN`
> **Category:** OO Modeling

Implements a **bidirectional association** between objects where one entity relates to many others, and the relationship is maintained consistently on both sides (no orphaned references).

**Key concept:** When object A references object B, object B must also reference object A — and this invariant is enforced programmatically.

**Use case:** Modeling teacher-student, parent-child, or team-member relationships in object-oriented systems.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Java (JDK 8+) |
| Paradigm | Object-Oriented Programming |
| Build | `javac` / IDE (IntelliJ, Eclipse) |
| Tests | Manual / JUnit (optional) |

---

## 🚀 Getting Started

### Prerequisites

- [Java JDK](https://adoptium.net/) 8 or higher
- An IDE (IntelliJ IDEA, Eclipse, VS Code) or a terminal

---

### Compile & Run

Navigate into any pattern folder and compile with `javac`:

```bash
# Compile all .java files in the folder
cd DESIGN_PATTERN_Strategie
javac *.java

# Run the main class
java Main
```

> Replace `Main` with the actual entry-point class name if it differs.

---

### With an IDE

1. Open the project root in **IntelliJ IDEA** or **Eclipse**
2. Navigate to any pattern folder
3. Right-click on the `Main.java` file → **Run**

---

## 📚 Design Pattern Reference

| Pattern | Category | Intent |
|---------|----------|--------|
| Adapter | Structural | Convert an incompatible interface into the expected one |
| Composite | Structural | Compose objects into tree structures for part-whole hierarchies |
| Observer | Behavioral | Notify dependents automatically on state change |
| Strategy | Behavioral | Encapsulate and swap algorithms at runtime |
| Mediator | Behavioral | Centralize complex communications between objects |

---

## 🧠 Concepts Covered

| Topic | Description |
|-------|-------------|
| SOLID Principles | Single Responsibility, Open/Closed, Liskov, Interface Segregation, Dependency Inversion |
| OOP Pillars | Encapsulation, Inheritance, Polymorphism, Abstraction |
| Interfaces & Abstract Classes | Used extensively across all patterns |
| Delegation | Core mechanism in Strategy and Adapter |
| Loose Coupling | Enforced through Mediator and Observer |
| Bidirectional Relations | Symmetric 1-to-N consistency management |

---

## 🤝 Contributing

1. Fork the project
2. Create your branch (`git checkout -b feature/new-pattern`)
3. Commit your changes (`git commit -m 'Add Singleton pattern'`)
4. Push to the branch (`git push origin feature/new-pattern`)
5. Open a Pull Request

---

## 👤 Author

**Yannis Duvignau**  
[GitHub](https://github.com/yannisduvignau)

---

## 📄 License

This project is distributed under an open license. See the `LICENSE` file for more details.