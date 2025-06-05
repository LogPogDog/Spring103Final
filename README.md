# Spring103Final

Dependencies:

Main control CPX boards from Adafruit: [https://github.com/adafruit/Adafruit_CircuitPlayground]
AsyncDelay: [https://github.com/stevemarple/AsyncDelay]
Wire.h: [https://docs.arduino.cc/language-reference/en/functions/communication/wire/]
SPI.h: [https://docs.arduino.cc/language-reference/en/functions/communication/SPI/]


Game Description

CPX Rhythm is a game that recreates the experience of classic video games like Piano Tiles, Geometry Dash, and much more that depend on a good sense of music and time. One song will be available for the final demo, which is Spear of Justice by Toby Fox

Rules/Scoring

The goal of the game is to be as accurate as possible with pressing the buttons when indicated. LEDS will light up and appear to move toward the top of the CPX board on either side of the board, and the player must hit the corresponding button at the appropriate time. Music will also be playing. There are 3 categories of score that you can receive for each button press: “Great” (when the button is pressed +/- 100 ms of the desired time, gives 300 points), “Okay” (within +/- 200 ms, gives 100 points), and “Miss” (any other time during the song, subtracts 100 points). The player is encouraged to go for a high score, and if they get all Greats, they achieve a “PERFECT” run! These are the only rules. There will also be a pause option where the player can exit the song. At the end of the game, the board will announce the score.
In addition, there will be 3 difficulties: Easy, Hard, Demon. Difficulty levels are distinguished by how many notes the player has to play in the song (Demon is ALL the notes, Easy is just the essentials). In the main menu, the player can choose their difficulty before entering the song.

Inputs

Switch: The switch distinguishes between “in-game” versus “out-of-game.” IMPORTANT: The switch should start in the OFF position. In this initial OFF position, the player can select their difficulty in the main menu. If the switch is placed in the ON position, the player will enter the song and play as usual. If at any point during the game the switch is placed in the OFF position, the game will “pause.” The player then has 3 options: Resume the game (switch back to ON position), Restart the game (hit the left button), or Go back to main menu (hit the right button).
Buttons: Both buttons provide similar functionality depending on the context. In the main menu, buttons cycle through the difficulties one at a time (left goes left, right goes right). In game, the buttons are solely used for presses. Left button inputs a “left press” while right button inputs a “right press.” Finally, as described above, they are used in the pause.

Outputs
LEDS: Lights are crucial to this game. They distinguish difficulty levels in the main menu, and they also provide indicators of when to press which buttons. LEDs are also used in the win screen to celebrate completion.
Sound: Sound is also crucial. Spoken instructions and scores will be used as much as possible. Sound is mostly used for the song component of the game.
	
