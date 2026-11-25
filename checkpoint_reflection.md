# Nikhil Wadia
## Reactor Operator: A Nuclear Power Plant Simulator
## A text-based C++ game where the player runs a pressurized water reactor (PWR) for 30 days. Each day the player sets the control rods and coolant pump speed to meet the grid's power demand without overheating the core. Random events are read from a file, and the game saves progress, writes a daily operator log, and keeps a top-10 leaderboard.

---

## checkpoint-01: Initial project structure / setup

1. What challenges did you encounter?

   Getting g++ to build more than one .cpp file at once. By default the VS Code build task only compiles the file that is open, so I updated tasks.json to use "*.cpp" so every source file in the folder gets compiled together.

2. What design decisions or changes did you make?

   I set up the files to match my Phase II design. Each class (Reactor, Operator, Event) has its own header (.h) and source (.cpp) file. I made five data files: reactors.txt and events.txt are read in, savegame.txt and leaderboard.txt are read and written, and operator_log.csv is written. The files are empty for now. main.cpp only prints Hello World to confirm the compiler works.
