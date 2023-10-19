Multi-color LED Controller for KL25Z
This project provides a system to control the on-board LEDs of the Freedom KL25Z board. Separate state machines are implemented for each of the Red, Green, and Blue LEDs, allowing them to flash at different intervals.

Features
Individual control of Red, Green, and Blue LEDs using separate state machines.
Red LED blinks with a pattern of 5 seconds ON and 5 seconds OFF.
Green LED blinks with a pattern of 3 seconds ON and 3 seconds OFF.
Blue LED, as an example, blinks with a pattern of 4 seconds ON and 4 seconds OFF.



Requirements
Freedom KL25Z development board.
Keil uVision or any compatible IDE for building and flashing the program.
The provided gpio.h header file.


Setup
Connect the Freedom KL25Z board to your computer.
Open the project in your preferred development environment.
Build the project.
Flash the compiled program to the KL25Z board.



Usage
Once flashed, the onboard LEDs will start blinking based on the specified patterns for each color.

File Descriptions
main.c: Contains the main program, initialization functions, and separate state machines for controlling each LED.
SysTick.c and SysTick.h: Provide functionality for system ticks, which are used for time delays.
gpio.h: Contains macro definitions related to GPIO pins and LED configurations.


Modification
To adjust the blinking pattern of each LED:

Find the respective Task[Color] function in main.c.
Modify the count[Color] values to adjust the ON and OFF times.
Rebuild and reflash the program to the KL25Z board.