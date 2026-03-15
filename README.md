
# Wellness App - Java OOP Project

A comprehensive **Wellness Tracking Application** built using **Java Swing**, demonstrating **Object-Oriented Programming (OOP)** concepts. The app allows users to track fitness, meals, habits, and health metrics through an interactive GUI.

---

## Table of Contents

- [Features](#features)  
- [OOP Concepts Used](#oop-concepts-used)  
- [Tech Stack](#tech-stack)  
- [Project Structure](#project-structure)  
- [Setup Instructions](#setup-instructions)  
- [Usage](#usage)  
- [Data Storage](#data-storage)  
- [Screenshots](#screenshots)  
- [Notes](#notes)  

---

## Features

### 1. User Management
- Create new accounts and login
- Store user information (username, password, height, weight)

### 2. Fitness Tracking
- Track daily steps
- Record workout types and calories burned
- Track sports activities
- Set and monitor daily targets
- “New Day” button resets daily metrics

### 3. Meal Tracking
- Add meals with calorie info
- Track water intake
- Set daily calorie and water targets
- View history of meals
- “New Day” resets data

### 4. Habit Tracking
- Create, toggle, and remove habits
- Track habit completion
- “New Day” resets habit completion

### 5. Health Calculators
- BMI (Body Mass Index)
- BMR (Basal Metabolic Rate)
- TDEE (Total Daily Energy Expenditure)

### 6. Dashboard
- Visual overview of:
  - Steps vs target
  - Calories burned vs target
  - Water intake vs target
  - Calories consumed vs target

---

## OOP Concepts Used
- **Classes & Objects:** User, FitnessData, MealData, Habit, HabitTracker  
- **Inheritance:** Comparable interface  
- **Polymorphism:** Interface implementations, method overriding  
- **Encapsulation:** Private fields with getters/setters  
- **Static Methods:** Validator, Calculator, FileHandler (Singleton)  
- **Collections:** ArrayList, HashMap  
- **Exception Handling:** Custom exceptions, try-catch blocks  
- **File Handling:** Serialization for persistence  
- **GUI Components:** Swing (JFrame, JPanel, JButton, etc.)  
- **Event Handling:** ActionListeners  
- **Design Patterns:** Singleton (FileHandler), Composite (GUI structure)  

---

## Tech Stack
- **Language:** Java  
- **GUI:** Java Swing  
- **Data Persistence:** File serialization (.dat files)  
- **IDE:** Visual Studio Code / IntelliJ IDEA  

---

## Project Structure
fitpro/
├── src/
│   └── wellnessapp/
│       ├── exceptions/
│       │   └── InvalidInputException.java
│       ├── models/
│       │   ├── User.java
│       │   ├── FitnessData.java
│       │   ├── MealData.java
│       │   ├── Habit.java
│       │   └── HabitTracker.java
│       ├── utils/
│       │   ├── Validator.java
│       │   ├── Calculator.java
│       │   └── FileHandler.java
│       ├── gui/
│       │   ├── LoginFrame.java
│       │   ├── MainFrame.java
│       │   ├── Dashboard.java
│       │   ├── FitnessPanel.java
│       │   ├── MealPanel.java
│       │   ├── HabitPanel.java
│       │   └── CalculatorPanel.java
│       └── main/
│           └── Main.java
└── README.md
---

## Setup Instructions

### Compile

```bash
# Navigate to project root
cd fitpro

# Compile all Java files
javac -d bin src/wellnessapp/**/*.java
Run
# Run main class
java -cp bin wellnessapp.main.Main

On Windows CMD:

java -cp bin wellnessapp.main.Main
