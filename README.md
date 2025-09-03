# Tic-Tac-Toe-
🎮 Tic-Tac-Toe – Low-Level Design (LLD) with Java
This project demonstrates the application of Low-Level Design (LLD) principles, Java OOP concepts, SOLID design principles, and design patterns.

The case study used here is Tic-Tac-Toe, which serves as a familiar problem domain to illustrate how requirements can be translated into UML models, classes, and responsibilities before implementation.
<img width="81" height="80" alt="{A3C6B5E9-A27D-4366-A1F3-12732B01B615}" src="https://github.com/user-attachments/assets/56cddb8d-73b2-46fe-9a60-12e51f064954" />


🔎 General Concepts
🔹 Object-Oriented Programming (OOP) in Java

Encapsulation → grouping attributes & methods inside classes (e.g., Board, Player).

Abstraction → exposing only essential behavior (e.g., makeMove() without revealing internals).

Inheritance → enabling extension (e.g., HumanPlayer vs AIPlayer).

Polymorphism → allowing different behaviors (e.g., multiple validation strategies).

🔹 Low-Level Design (LLD)

LLD focuses on bridging requirements and implementation through structured design:

Requirement Analysis

Use Case Definition

NVT Technique (Narrative → Visual → Textual)

UML Diagrams (Use Case, Class, Sequence)

Class & Object Design

Responsibility Assignment

🔹 SOLID Principles

Single Responsibility → each class handles one concern (Board vs Validator).

Open/Closed → extendable for AI mode or larger boards without major changes.

Liskov Substitution → AIPlayer can replace HumanPlayer seamlessly.

Interface Segregation → classes expose only necessary operations.

Dependency Inversion → higher-level modules (Game) depend on abstractions.

🔹 Design Patterns

Factory Method → to create different types of players.

Strategy → for move validation or win-checking rules.

Singleton → for managing a single instance of GameController.

📌 Case Study: Tic-Tac-Toe

Tic-Tac-Toe is chosen as a demonstrative example for LLD because it has:

Clear rules

Defined interactions

Simple yet extensible requirements

This makes it ideal to showcase design principles without unnecessary complexity.

📋 Requirement Analysis

Two players (X and O).

A 3x3 board to record moves.

Validation for legal moves.

Win/draw detection.

Support for restart/future extension (AI, custom board size).

🔑 Use Cases

Start a new game.

Player makes a move.

Validate move and update board.

Check for winner or draw.

Restart game.

🧩 NVT Technique

Narrative → “A player selects a cell. If valid, the mark is placed. If win/draw occurs, the game ends.”

Visual → UML Diagrams (Use Case, Class, Sequence).

Textual → Java classes and methods derived from UML.

🏗️ UML Diagrams

Use Case Diagram → Player ↔ Game ↔ Board.

Class Diagram → Game, Board, Player, Cell, Validator.

Sequence Diagram → Flow of a player move through system interactions.

🖥️ Class & Object Design
Classes

Game → Controls flow of play.

Board → Maintains the 3x3 grid.

Player → Abstract class for HumanPlayer and AIPlayer.

Cell → Represents state of a board position (X, O, Empty).

Validator → Encapsulates rules for win/draw.

Responsibilities

Game → Orchestrates gameplay.

Board → Updates and tracks state.

Player → Holds identity & move logic.

Cell → Atomic unit of play.

Validator → Applies rules and checks outcomes.

🎯 Goal

To demonstrate the systematic process of LLD: requirement analysis → use cases → UML → class design → implementation.

To apply Java OOP, SOLID principles, and design patterns in a practical case study.

To create a design that is modular, extensible, and maintainable.

To showcase an LLD approach generalizable to other problem domains, with Tic-Tac-Toe as the example.
