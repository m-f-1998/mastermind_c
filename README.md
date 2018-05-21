# Mastermind Game on Raspberry Pi

### Created by Matthew Frankland (March 2018)
### Source Code Locked Due to Similarities with Current Coursework. Email mf48@hw.ac.uk to Request Password.

## Problem Specification

This task involved developing an implementation of the classic board game MASTERMIND in both C and Assembler using hardware wiring techniques. The main problem of this coursework was using hardware components, such as LEDs; an LCD; and a Button, to accept user input rather than direct interaction with the terminal.

MASTERMIND is a game between two players, one player who uses N pegs of C colours to create a secret order, and another who is tasked with guessing the secret order within a restricted number of guesses. At the end of each round the guesser is informed: how many pegs are of the right colour and position; and how many pegs are of the right colour but not in the right position.

To keep the logic simple, a decision was made to only use 3 pegs of three different colours. Our goal in this task was to use the button to accept a number between 1 and 3 (to represent colours) and store this in a fixed length array (to represent order). This array could then be manipulated using the program logic and relevant information outputted to the LCD.

## Hardware Specification:

Hardware components for this coursework included a breadboard, an LCD, a button, and two LEDs (one red and one yellow), all of which were connected to Raspberry Pi 2 using wires and resistors where necessary. All appropriate hardware components are memory mapped so that they can be manipulated by writing to memory.

The GPIO connections for this coursework are listed below:
    • REDLED-GPIO5
    • YELLOW LED - GPIO 13
    • BUTTON - GPIO 19
    • REGISTER SELECT (LCD 4) - GPIO 25
    • ENABLE (LCD 6) - GPIO 24
    • DATA CABLE 1 (LCD 11) - GPIO 23
    • DATA CABLE 2 (LCD 12) - GPIO 10
    • DATA CABLE 3 (LCD 13) - GPIO 27
    • DATA CABLE 4 (LCD 14) - GPIO 22
