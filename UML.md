UML Class Diagram 
![UML](https://github.com/user-attachments/assets/a22fbd7f-1b46-448d-a601-6d95d14ded27)
Game → Central controller that manages players, board, rules, and notifications.

Board → Maintains the grid state and provides operations for marking and displaying cells.

Player → Represents a user with id, name, symbol, and score.

Rule (Strategy) → Abstract class for game rules. StandardRule implements logic to decide winners/draws.

Notification (Observer) → Handles in-app and external notifications when moves are made or results are declared.

GameFactory → Creates and returns game objects based on type (e.g., standard).

Design Highlights

Strategy Pattern → for flexible rule definitions.

Observer Pattern → for app and external notifications.

Factory Pattern → for decoupled game creation.

Board is n × n and supports constraints (no diagonal wins).
