---
draft: false
title: 'Pirate Wars C Battle Simulation'
summary: "A multi-threaded battle simulation in C"
cover:
  image: PirateWars.png
  alt: "A pic of the project code"
  relative: false 
---

## Overview

This project was the final in my systems programming course. A course which taught me many programming fundamentals extendable past C. All our coursework was done within a Ubuntu Linux VM, which familiarized me with the operating system. 

The purpose of the project is to simulate a battle where two heroes, a tortoise and a hare, fight a crew of pirates. They only have one magical sword, which increases the wielder's strength. This program simulates the possible outcomes of success, partial success, and failure for each scenario: the tortoise has the sword, the hare has the sword, and no one has the sword. It accumulates statistics and prints to the user the percentage each outcome has occurred for each scenario based on the number of runs.

### Code

Check out the github [repository.](https://github.com/TheNoahProdigy/PirateWarsCBattle)

#### File Structure

_defs.h_ is a header file containing all:
- #includes to external libraries
- Constant definitions
- enums
- struct definitions
- function prototypes

_main.c_ facilitates the program's control flow, and all other source files group function definitions by context.

#### Data Structures
This program utilizes a custom deque data structure, which stores the pirates, enabling the heroes to fight the pirates from both sides simultaneously in different threads.

Several C-Structs and C-Arrays are used to store data both dynamically and statically. 

#### Memory Managment

#### Threads

Multiple threads are spun up by leveraging the pthreads library, and using the semaphore library ensures data synchronization. 


### Demo


---

## Execution Instructions

---

## Tech Stack
- C
- Make files

