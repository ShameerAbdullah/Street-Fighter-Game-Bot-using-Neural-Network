
# AI PROJECT PART 2
This README provides detailed instructions on how to set up and run the provided code solution for the tournament game. Please follow the steps below to install the necessary dependencies and execute the code successfully on your machine.
## Prerequisites/Dependencies:
- Operating System: Windows 7 or above (64-bit)
- Python version 3.6.3 or above (Note: The code has been tested on version 3.6.3 but should work on higher versions of Python. For versions below 3, minor modifications may be required.)
- Prerequisites for the BizHawk emulator. 
## Installation and Setup:
- Extract the contents of the attached zip file to a preferred location on your machine.
- Install Python 3.6.3 or a higher version if not already installed on your system. You can download Python from the official website (https://www.python.org/downloads/).
- Install the numpy library for the game by running the following command in the command prompt or terminal:
Pip install numpy
- Once the dependencies are installed, navigate to the folder based on your requirement:
For running a single bot (your bot vs CPU), open the "single-player" folder.
For running two of your bots simultaneously (both fighting each other), open the "two-players" folder.

## Running the Game and Executing the API Code:
- Open the "EmuHawk.exe" file located in the BizHawk emulator folder.
- From the "File" drop-down menu in the emulator, choose "Open ROM" or use the shortcut "Ctrl+O".
- Browse to the respective folder (single-player or two-players) and select the "Street Fighter II Turbo (U).smc" file.
- From the "Tools" drop-down menu in the emulator, open the "Tool Box" or use the shortcut "Shift+T".
- Leave the emulator window and the tool box open, then open the command prompt or terminal and navigate to the directory where the API code is located.
- Run the following command in the command prompt or terminal to execute the Python API code:
	python controller.py 1
Note: The '1' at the end of the command is a command-line argument. Use '1' to control player 1 (left-hand side player in the game) through your bot. If you want to control player 2 (right-hand side player in the game), use '2' as the command-line argument. Any other command-line argument will result in an error.
- After executing the code, go to the emulator window and select your character(s) in the game after choosing the normal mode. You can configure the controls for selecting players from the "Controllers" option in the "Config" drop-down menu of the emulator.
- In the emulator, click on the second icon in the top row (Gyroscope Bot). This action will establish a connection between the emulator and the API program. You should see the message "Connected to the game!" or "CONNECTED SUCCESSFULLY" in the terminal or command prompt.
- If you have successfully completed all the steps above, you have now successfully run the GameBot starter code.
- The program will stop once a single round is finished. To run the emulator and the code again, repeat the process from Step 1.
- To run two bots at the same time and make them fight each other, run both your bots simultaneously with different command-line arguments. Use '1' for the first and '2' for the second bot. Open two instances of the command prompt or terminal, navigate to the directory where the API code is located, and run the following commands in each instance:
	For Bot 1:
		python controller.py 1
	For Bot 2:
		python controller.py 2
- Additionally, in the game (emulator window), make sure to select the "VS Battle" mode and choose two players.
- Repeat the previous steps for running the emulator and the code to initiate the battle between the two bots.

Congratulations! You have successfully set up and executed the tournament GameBot on your machine. Good luck in the tournament!


