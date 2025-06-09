# Spring103Final - Logan McClure

Game Demo: [https://youtu.be/eawExi77x0I]

Dependencies:

Main control CPX boards from Adafruit: [https://github.com/adafruit/Adafruit_CircuitPlayground]
AsyncDelay: [https://github.com/stevemarple/AsyncDelay]
Wire.h: [https://docs.arduino.cc/language-reference/en/functions/communication/wire/]
SPI.h: [https://docs.arduino.cc/language-reference/en/functions/communication/SPI/]


Game Description

CPX Rhythm is a game that recreates the experience of classic video games like Piano Tiles, Geometry Dash, and much more that depend on a good sense of music and time. One song will be available for the final demo, which is Spear of Justice by Toby Fox

Rules/Scoring

The goal of the game is to be as accurate as possible with pressing the buttons when indicated. LEDS will light up and appear to move toward the top of the CPX board on either side of the board, and the player must hit the corresponding button at the appropriate time. Music will also be playing. There are 3 categories of score that you can receive for each button press: “Great” (when the button is pressed +/- 55 ms of the desired time, gives 300 points), “Okay” (within +/- 110 ms, gives 100 points), and “Miss” (any other time during the song, subtracts 100 points). The player is encouraged to go for a high score. These are the only rules. At the end of the game, the board will announce the score.

Inputs

Buttons: Both buttons provide similar functionality. In-game, the buttons are solely used for presses. Left button inputs a “left press,” while right button inputs a “right press.”

Outputs

LEDS: Lights are crucial to this game since they provide indicators of when to press which buttons. Blue LEDS represent upcoming notes, Red represents a "miss," Yellow represents "okay," and Green represents "great."
Sound: Sound is also crucial. Spoken scores will be used at the end of the game, and otherwise sound is used for the song component of the game.
PrintOuts: The player can view their score changing in real time with the serial monitor. Every button press modifies the score, and it will print "GREAT!", "Okay!", or "Miss!" depending on the press.
	
