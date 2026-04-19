# guard-logic-game (C++)

> A mini project demonstrating a randomized decision-making system using Object-Oriented Programming in C++.

---

## 🚀 Overview

This project simulates a simple guard-based decision system in the form of a command-line game.

The user is presented with three doors:
- Safe Exit ✅
- Trap ❌
- Back to Start 🔁

Unlike a fixed system, the outcomes of these doors are randomized in every round. This removes predictability and makes the system more realistic.

Additionally, a guard mechanism is introduced:
- When the guard is active, the user is forced back to the starting point regardless of their chosen door.

The game runs for a limited number of attempts and provides options to restart or exit after completion.

---

## 🧠 Problem Approach

Instead of using static conditions, the system is designed with **dynamic decision-making**:

1. **Randomization**
   - Door outcomes are shuffled each round using `std::shuffle`
   - Ensures unpredictability

2. **Guard Logic**
   - A random guard condition overrides user choice
   - Simulates external constraints in decision systems

3. **Controlled Attempts**
   - The user gets a fixed number of attempts (default: 3)
   - Adds challenge and structure

4. **State Management**
   - Game state is reset properly on restart
   - Ensures consistent behavior

---

## 🧱 System Design (OOP)

The entire logic is encapsulated inside a `Game` class:

- `shuffleDoors()` → Randomizes door positions  
- `isGuardActive()` → Simulates guard condition  
- `getUserChoice()` → Handles input validation  
- `askRestart()` → Controls replay flow  
- `play()` → Main game loop  

This design improves:
- Code readability  
- Maintainability  
- Scalability  

---

## 🧩 Features

- 🎲 Randomized door allocation  
- 🚨 Guard-based override logic  
- 🔁 Retry system with limited attempts  
- ♻️ Restart & Exit options  
- ✅ Input validation  
- 🧱 Clean OOP structure  

---

## 🛠️ Technologies Used

- C++
- STL:
  - `vector`
  - `algorithm`
  - `random`

