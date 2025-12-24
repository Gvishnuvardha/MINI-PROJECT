# MINI-PROJECT
Smart Car System is a Java-based mini project developed using Core Java and OOPS concepts. It applies the Strategy Design Pattern to dynamically switch engine behavior at runtime, achieving loose coupling, scalability, and maintainable code structure suitable for real-world applications


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Smart Car System – Core Java Mini Project

## Description
Smart Car System is a Core Java mini project that demonstrates Object-Oriented Programming
concepts and the Strategy Design Pattern. The project models a car system where engine
behavior can be changed dynamically at runtime.

## Features
- Runtime engine switching (Power Engine ↔ Electric Engine)
- Media control system (start/stop music)
- Brake system implementation
- Loose coupling using interfaces

## Technologies Used
- Java (Core Java)
- OOPS Concepts
- Strategy Design Pattern

## OOPS Concepts Used
- Abstraction (Interfaces)
- Encapsulation
- Polymorphism (Runtime)
- Composition (HAS-A relationship)

## Design Pattern
- Strategy Pattern

## How to Run
1. Clone the repository
2. Compile the code in online java compiler files
3. Run the code

## Sample Output
Power engine starts  
Power engine accelerating  
Music started  
Engine upgraded to Electric Engine  
Electric engine starts  
Brake applied

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                           (UML DESIGN)

            <<interface>>
              Engine
          ----------------
          + start()
          + stop()
          + acc()
               ▲
      -----------------------
      |                     |
PowerEngine           ElectricEngine
----------------     ----------------
+ start()             + start()
+ stop()              + stop()
+ acc()               + acc()


            <<interface>>
              Media
          ----------------
          + start()
          + stop()
               ▲
               |
          ----------------
            CdPlayer
          ----------------
          + start()
          + stop()


            NiceCar
--------------------------------
- engine : Engine
- player : Media
--------------------------------
+ start()
+ stop()
+ acc()
+ startMusic()
+ stopMusic()
+ upgradeEngine()
