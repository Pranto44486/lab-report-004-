# LabReport04 – GUI Development using Java Swing

This repository contains the solution for **LabReport04**, which demonstrates **GUI development in Java using the Swing framework**. The application allows the user to draw a filled circle at a random position and clear the drawing using buttons.

---

## Lab Objective

The objectives of this lab are to:
- Understand Java Swing components
- Implement event handling using `ActionListener`
- Perform custom drawing using `Graphics`
- Update the GUI dynamically based on user interaction
- Clear and redraw components correctly

---

## Concepts Covered

- Java Swing
- GUI Components (`JFrame`, `JPanel`, `JButton`)
- Event Handling
- `ActionListener`
- Custom Painting (`paintComponent`)
- Random positioning
- `repaint()` method

---

## Problem Description

The application includes:
- A main window with two buttons: **Draw Circle** and **Clear**
- A drawing panel for rendering graphics

### Functional Requirements:
- Clicking **Draw Circle** draws a filled circle at a random position inside the panel
- Clicking **Clear** removes all drawings
- Event handling is implemented using `ActionListener`
- The panel updates correctly on every user interaction

---

## UML Class Diagram
    +----------------------+
    |  CircleDrawingGUI    |
    +----------------------+
    | - drawButton         |
    | - clearButton        |
    | - panel              |
    +----------------------+
    | + actionPerformed()  |
    +----------------------+

    +----------------------+
    |      DrawPanel       |
    +----------------------+
    | - x: int             |
    | - y: int             |
    | - DIAMETER: int      |
    +----------------------+
    | + drawCircle()       |
    | + clearPanel()       |
    | + paintComponent()   |
    +----------------------+

---

##  Source Files

- `CircleDrawingGUI.java` – Main GUI class and event handling
- `DrawPanel` (inner class) – Handles drawing and clearing circles

---

##  How to Run the Program

1. Clone the repository:
   ```bash
   git clone <your-repository-link>
2. Compile the program:
 javac CircleDrawingGUI.java
3.Run the application:
java CircleDrawingGUI


