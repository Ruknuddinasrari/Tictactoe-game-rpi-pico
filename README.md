# Tictactoe-game-rpi-pico
Tic Tac Toe Game  on RPI Pico in C


![2](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/aae0dcda-ff30-4c2f-b1ec-134261c67340)


Description:
This project involves creating a Tic Tac Toe game that runs on the Raspberry Pi Pico using the C programming language. The game allows two players to compete in the classic game of Noughts and Crosses on a 3x3 grid, with the objective of aligning three of their respective symbols in a row.

Technical Details:
- Edge Detection: Implemented single pulse edge detectors to identify state changes in signals, crucial for button press recognition.
- Debouncing: Utilized software debouncing techniques to ensure clean, bounce-free button inputs.
- Multicore Processing: Leveraged the Pico's multicore functionality for efficient task handling and parallel processing.

Hardware Components:
- Raspberry Pi Pico
- Breadboard
- LEDs (Red & Green)
- 330 Ω Resistors
- Push Buttons (x3)
- Jumper Wires (Male-to-Male)

Software Tools:
- GNU Arm Embedded Toolchain
- Mingw-w64
- CMake
- Visual Studio Code
- Git for Windows
- PuTTY

Gameplay Mechanics:
Players use push buttons to select grid cells and confirm their moves. The game tracks player turns and symbol placements, checking for win conditions or a draw. LED indicators provide visual feedback for player turns and game outcomes.

Code Structure:
The codebase includes functions for GPIO initialization, button state management, and game logic. The `init_gpio` function sets up the GPIO pins, while the `debounce` function handles button press validation.

Conclusion:
This project served as an excellent learning experience in embedded systems design, particularly in understanding the Pico's capabilities and implementing effective input handling techniques.

![image](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/f6780f34-3648-4c17-970e-601448f62edb)


![image](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/5606b53b-2e56-4a41-9afc-a780ff1e8603)



![3](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/89a2ae70-c501-4284-b869-6a57173a8487)
