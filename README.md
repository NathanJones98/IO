# IO
A Lab for ECE243

# Part 1:
Objective: Implement a simple program that reads key presses from an input device and displays corresponding values on a seven-segment display.
Initialization: Initializes memory addresses for the seven-segment display (HEX_ADDR), the key input (KEY_ADDR), and a lookup table for displaying numbers on the seven-segment display (HEX_BITS).

Main Loop:
Reads the value of the key input.
Waits for a key press (waits until the key input value is non-zero).
Determines which key was pressed (KEY0, KEY1, KEY2, or KEY3).
Performs actions based on the pressed key:
KEY0: Resets the display to zero.
KEY1: Increases the display value by 1.
KEY2: Decreases the display value by 1.
KEY3: Clears the display and waits for another key press.
Continues the loop.

# Part 2:
Objective: Implement a program that counts up continuously and resets when a specific edge is detected on an external signal.
Initialization: Similar to Part 1, initializes memory addresses for the display (HEX_ADDR), the edge detection signal (EDGE_ADDR), and the lookup table for displaying numbers (HEX_BITS).

Main Loop:
Delays execution.
Increments the count.
Checks for an edge on the external signal.
If an edge is detected, clears the display and restarts the count.
Displays the count on the seven-segment display.
Continues the loop.

# Part 3:
Objective: Similar to Part 2 but introduces additional functionality for interacting with a timer.
Initialization: Initializes memory addresses for the display (HEX_ADDR), the edge detection signal (EDGE_ADDR), and a timer (TIMER_ADDR), in addition to the lookup table for displaying numbers (HEX_BITS).

Main Loop:
Delays execution using a timer.
Increments the count.
Checks for an edge on the external signal.
If an edge is detected, clears the display and restarts the count.
Displays the count on the seven-segment display.
Continues the loop.

Additional Notes:
The code heavily utilizes load and store instructions to read and write data from/to memory-mapped hardware registers.
It employs branching instructions (BEQ, BNE, B, BL, etc.) to control program flow based on conditions.
It uses a combination of predefined constants, lookup tables, and arithmetic operations to manipulate data and perform desired actions.
The code also manages resources such as timers and external signals to synchronize operations and respond to external events.





