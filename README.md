Bagels: a guessing game 
----
Implemented by Alan Au

Code was (mostly) written at Seattle PyLadies EastSide hack night on 2017-11-06.

----
The game will generate a 3-digit non-repeating number from digits 0-9.

The player will enter a 3-digit guess, and the game will respond as follows:
- 'Fermi'  = correct digit in proper place
- 'Pico'   = correct digit in wrong place
- 'Bagels' = no correct digits

----
The player can receive multiple responses, e.g. 'Fermi Pico' means both apply.

The order of responses doesn't correspond to the order of the guessed digits. 
e.g. 'Fermi Pico Pico' doesn't mean 'Fermi' applies to the 1st guessed digit.

When the player guesses all 3 digits in the correct positions, the game will 
respond 'Fermi Fermi Fermi' and report how many valid guesses were made.

Players may also request a "hint" which will report any digits that the player
knows have been ruled out (by a 'Bagels' response).

Players may request the "answer" to reveal the answer and end the current game.

Players may also quit immediately using the "exit" or "quit" commands.
