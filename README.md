# BTD6 Automation Template
**Status:** Functional Template / Portfolio Piece  
**Language:** Python (PyAutoGUI, PyDirectInput)

## Overview
This project is a modular framework designed to automate BTD6 gameplay loops. It represents a shift from rigid, hard-coded scripting toward a dynamic, state-aware system that is easier to maintain and scale.

## Technical Features
* **Resolution Independence:** Uses coordinate ratios (`widthRatio`, `heightRatio`) to scale mouse movements and clicks dynamically. This allows the script to function across different monitor resolutions (e.g., 1080p to 4K) without recalibration.
* **State Management:** Utilizes Dictionaries and Lists to track the real-time status of placed towers. The framework "remembers" placed monkeys and their current upgrade levels to inform future logic.
* **Upgrade Logic:** Implements an algorithm that compares current entity states against a target upgrade path (e.g., `3-0-2`). It calculates the exact number of inputs required, ensuring the right upgrades are chosen.
* **Functional Abstraction:** Separates core logic from input execution. By wrapping interactions into standardized functions (e.g., `PlaceMonkey`, `UpgradePath`), the system is more modular and easier to debug.

## Project Evolution
The repository includes `Egg and Spoon Race Macro.py` as a legacy reference. Comparing it to `FunctionsTesting.py` demonstrates the transition from procedural, coordinate-locked scripting to a flexible, data-driven architecture.
