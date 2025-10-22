---
draft: false
title: 'Oasis Pro Software'
summary: "Software for a medical device in Qt C++"
weight: 2
cover:
  image: OasisPro.png
  alt: "C++ Device Code"
  relative: false 
---

## Overview

This project was the final assignment for a third-year software engineering course I took during my undergraduate studies. It taught/reinforced OOP principles and common design patterns. This course is the conclusion of a string of OOP-centric development classes, all of which taught me software development skills in several languages (Python, Java, C++). Through this breadth of exposure, I learned the fundamental software engineering skills which transcend a particular language.

My group (_Antwan Gad, Jesse Mendoza, Tristan Turner, Victoria Nguyen_) and I developed this medical device software in C++ using the Qt framework. It's designed to fulfill a set of requirements similar to what a client would provide in a contract.

### Documentation

If you're curious about the documentation [here](OasisProDocumentation.pdf) you can find the main use case, UML diagrams, how to test section, and more.

### System Architecture 

The system architecture is divided into two primary components:
- Backend (Device Layer): Manages the device’s internal logic, including session handling, user management, and state control
- Frontend (MainWindow Layer): Provides a Qt-based GUI through which users could interact with the simulated device, altering internal states and observing system feedback in real time

### Design Best Practices & OOP Principles 

- Encapsulation:
  Core functionalities in Session, User, and Device are privatized to enforce internal handling and reduce coupling.

- Abstraction:
  High-level objects like Device, User, and Session encapsulate their own data and behavior, mirroring real-world entities and clarifying the codebase.

- Modularity & Layered Architecture:
  A dedicated interface layer connects backend logic to the GUI, isolating presentation from logic and enabling independent development and testing.

- State Management:
  Device state uses Boolean flags and float values (e.g., battery percentage), updated dynamically through user interaction and simulated device activity.

- Simulation & Real-Time Behavior:
  QTimer objects simulate time-dependent processes like battery depletion, closely mimicking hardware behavior.

- Documentation & Verification:
  UML diagrams (sequence, activity, state) document system behavior, and a traceability matrix links requirements to implementation and tests, ensuring coverage and validation.

### Code

Check out the github [repository.](https://github.com/TheNoahProdigy/MedicalDeviceSoftware)

### Demo

{{< youtube  EH2gb4paxHE >}}

---

## Tech Stack
**Language & Framework:** C++ with Qt

**Architecture & Design**: Object-Oriented Programming, Modular Layered Design, UML Documentation

**State & Simulation**: QTimer for time-dependent behavior, Boolean and float variables for device state

**Testing & Verification**: Traceability matrix, functional test cases