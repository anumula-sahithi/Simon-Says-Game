# Simon Says Game

A simple and engaging project built using Arduino that replicates the classic "Simon Says" game. The game uses push buttons, buzzers, and LED lights for interaction, along with an OLED display to show the rules and score.

---

## Introduction
The "Simon Says" game challenges players to memorize and replicate sequences of lights. With each correct round, the sequence becomes one step longer, increasing the difficulty. This project utilizes Arduino to manage inputs, outputs, and logic, creating an interactive experience for players.

---

## Features
- *Interactive Gameplay:* Players press buttons corresponding to the LED lights to mimic the sequence.
- *Sound Feedback:* A buzzer provides audio feedback for correct and incorrect inputs.
- *Score Tracking:* An OLED display keeps track of the current score.
- *User Guidance:* The OLED displays the rules at the beginning and updates the score dynamically during gameplay.
- *Dynamic Difficulty:* The sequence grows progressively longer as the player succeeds.

---
## Additional Features
This game also has two modes:
- *Progressive mode:* If the player selects green, the game proceeds in progressive mode, where the sequences grow longer step by step as the levels increase, making the game gradually more challenging.
- *Random mode:* If the player selects red, the game proceeds in random mode, where the sequences change unpredictably at each level, testing the player's reflexes and memory under dynamic conditions.
---

## Components Used
- *Arduino UNO Board*
- *Push Buttons (4)*
- *LEDs (4)*
- *Resistors (appropriate values for LEDs and buttons)*
- *Buzzer*
- *OLED Display*
- *Breadboard and Jumper Wires*
- *Power Source (e.g., USB or battery pack)*

---

## How to Play
1. *Start the Game:* The OLED displays the game rules and waits for the player to press a button to begin.
2. *Select the game mode:* The OLED displays the modes and waits for the player to select a game mode to begin.
3. *Watch the Sequence:* LEDs light up in a sequence with corresponding buzzer sounds.
4. *Replicate the Sequence:* The player presses the buttons in the same order as the LEDs.
5. *Score Points:* The score increments for each correctly completed sequence.
6. *Game Over:* If the player inputs an incorrect sequence, the game ends, and the final score is displayed.

---

## Setup Instructions
1. *Hardware Assembly:*
   - Connect all components to the Arduino as per the circuit diagram.
   - Ensure proper connections for the OLED display (I2C pins).
   - Use the breadboard to organize components neatly.

2. *Upload Arduino Code:*
   - Install the necessary Arduino libraries (e.g., Adafruit SSD1306 and GFX libraries for the OLED).
   - Open the provided Arduino code in the IDE.
   - Select the correct board and port, then upload the code.

3. *Power On:*
   - Power the Arduino via USB to start the game.

---

## Arduino Code Overview
The Arduino code manages the following:
1. *Initialization:*
   - Configures the I/O pins, initializes the OLED display, and sets up variables for gameplay.
2. *Game Loop:*
   - Generates random sequences for the LEDs and buzzer.
   - Checks player inputs for correctness.
   - Updates the score and displays it on the OLED.
3. *Feedback:*
   - Controls the LEDs and buzzer for visual and audio cues.
   - Displays game over and score messages on the OLED.
