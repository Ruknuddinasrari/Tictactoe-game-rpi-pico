# Tictactoe-game-rpi-pico
Tic Tac Toe Game  on RPI Pico in C


![2](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/aae0dcda-ff30-4c2f-b1ec-134261c67340)

For this project I have used a Pico h, a breadboard; a red, and a green LED; two 330 Ω 
resistors; a selection of male-to-male (M2M) jumper wires, and 3 push buttons. 

The software used are -GNU Arm Embedded toolchain, Mingw-w64 for Windows native build 
Cmake, Visual Studio Code, Git for Windows, and Putty.

As we know Nougats and Crosses, also called Tic Tac Toe, is a pencil-and-paper game for two players. The objective of the game is to have three of your symbols in a row, either horizontally, vertically, or diagonally, before your opponent does. The game is played on a 3x3 grid, and each player takes turns marking a square with either an "X" or an "O." In the event that all squares are occupied, and there is no winner the game ends in a draw and if there is a winner the reset button is requested.

To create the Tic-Tac-Toe project, I began by constructing a 3x3 grid to represent the game 
board. I then initialized two variables to keep track of the current player (1 or 2) and their 
corresponding symbols (X or O). To select a cell, I utilized push button 1, and after choosing the desired cell, the user confirms their move by pressing push button 2. When it's player 1's turn, I turned on the green LED, and for player 2's turn, I turned on the red LED. After every move, I examined the board to determine if a player had won the game (having three symbols in a row vertically, horizontally, or diagonally). If a player had won, I flashed the corresponding LED (green for player 1, red for player 2). In the case that all the cells are occupied, and no player has won, the game results in a draw, and both the green and red LEDs flash. To reset the game, I used push button 3. I printed the updated board on the screen via a USB connection using a Putty terminal after each move. Additionally, I included a printed statement that notifies the user when a cell is already occupied, and their symbol is not placed in that cell, And I implemented a button debounce software to eliminate the bouncing of electrical contacts in a switch or button.

The function init_gpio carries out the initialization of a group of GPIO (General Purpose 
Input/Output) pins by performing the following steps:
Iterating through an array of GpioConfig structures (gpio) of length len.
For each GpioConfig structure in the array, it invokes the gpio_init function with the pin_number field as an argument. This initializes the designated GPIO pin.
Then, it calls the gpio_set_dir function with the pin_number field and the pin_dir field as 
arguments. This sets the direction of the specified GPIO pin as input or output.
The function debounce is a low-level hardware implementation used to eliminate electrical noise generated during a button press. It verifies whether the button state has altered (has_changed) and if the new state is consistent (is_stable). If both of these conditions are met, it returns true to signify a valid button press. If either of the conditions is not met, it returns false, indicating an invalid button press.


![image](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/62fa9911-5b1b-4697-a690-38d23a7c9313)

![3](https://github.com/Ruknuddinasrari/Tictactoe-game-rpi-pico/assets/49069833/89a2ae70-c501-4284-b869-6a57173a8487)
