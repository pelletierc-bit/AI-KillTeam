# Kill Team AI Opponent — Final Project

This project simulates a tactical AI opponent for a tabletop skirmish game.  
The AI makes decisions based on distance, terrain, movement rules, and combat interactions.  
It is designed as a Python final project demonstrating object‑oriented programming, decision logic, and user interaction.

---

## 🎮 Gameplay Overview

Each turn is divided into two phases:

### **1. Positioning Phase**
- You enter the distance to each of your player operatives.
- The AI automatically identifies the closest enemy operative.
- The AI decides whether to:
  - Advance
  - Retreat
  - Climb (climb height subtracts from movement)
  - Hold position
- Movement updates the range to the closest enemy.
- The phase repeats until someone is within 6" (shooting range).

### **2. Shooting Phase**
- The player chooses an AI operative to attack.
- The AI rolls armor saves and updates health/morale.
- The AI then shoots back at the closest player operative.
- Damage and deaths are handled interactively.

---

## 🧠 Features

### ✔ Start‑of‑Game Roll‑Off
Both sides roll a d6 to determine who goes first. Ties reroll.

### ✔ Closest‑Enemy Targeting
The AI always focuses the nearest player operative based on distances you enter each turn.

### ✔ Climbing Logic
If the AI climbs:
- Climb height is subtracted from its movement.
- Remaining movement is applied toward or away from the target.

### ✔ Encapsulated OOP Design
- `AIOperative` class handles stats, movement, climbing, shooting, and saves.
- `AITeam` manages multiple AI operatives.
- `PlayerTeam` manages player operatives.
- Getter/setter used for range tracking.

### ✔ Interactive Combat
- Player attacks include hit/miss and damage.
- AI attacks include hit rolls and randomized damage.
- Armor saves reduce or negate damage.

---

## 📁 Project Structure
Final-Project/
│
├── main.py
├── ai_operative.py
├── ai_team.py
├── player_team.py
└── README.md


---

## ▶️ How to Run

1. Install Python 3.10+  
2. Open a terminal in the project folder  
3. Run: main.py from Final project folder
4. Follow the prompts during gameplay.

---

## 📘 File Descriptions

### **main.py**
Controls:
- Turn order roll‑off  
- Positioning phase  
- Shooting phase  
- Distance input  
- AI decision flow  

### **ai_operative.py**
Defines the AI operative:
- Health, morale, aggression  
- Movement and climbing  
- Shooting and armor saves  
- Range getter/setter  

### **ai_team.py**
Creates and manages the AI team.

### **player_team.py**
Creates and manages the player team.

---


## 🎯 Purpose

This project demonstrates:
- Object‑oriented programming  
- Encapsulation (getter/setter)  
- Conditional logic  
- User input handling  
- Multi‑file Python project structure  
- Tactical decision‑making simulation  

It serves as the final project submission for the Python programming course.

---

## 🎥 Project Videos

### **Code Demo**
This video demonstrates the program running through a full round, including initiative, AI positioning, and shooting logic.

🔗 **Demo Video:**  
[ Demo](https://youtu.be/T8n9oVGWgw0)

### **Walkthrough Presentation**
This video is my 3–5 minute walkthrough explaining the project’s purpose, structure, core logic, challenges, and future improvements.

🔗 **Walkthrough Video:**  
[Walkthough](https://youtu.be/ab87G6DNyFg)

---

## 📝 Citations

All code, logic structures, and design decisions in this project were created by the author as part of a Python programming final project.  
This work represents original development, including:

- Object‑oriented class design  
- Game logic and turn structure  
- Movement, climbing, and distance calculations  
- Shooting and armor save mechanics  
- User interaction and input handling  
- Tactical decision‑making algorithms  

This project is © 2026 by the author.  
Unauthorized copying, distribution, or modification of this code without permission is prohibited.
