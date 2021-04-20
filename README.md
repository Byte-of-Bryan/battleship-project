# battleship-project

Program written by Bryan Morandi - 2021

This is a small project that uses a multidimensional list to create a simple battleship
game against an AI. The skills that I practiced in writing this program are: 
OOP, exception handling, and modularity.

The goal of the game is to sink the enemy battleship that is hidden, by
guessing row and column coordinates each turn. But be carful because the 
enemy also guesses coordinates and can sink your ship if you don't sink theirs first!

The sea is made up of a grid consisting of "O"'s these are currently empty slots
that either have the enemy ship that is hidden from the player, or can be attacked
either by the player or enemy. Once the player chooses coordinates for their ship,
their ship is represented by "#" this is then shown in the sea. When it is time for
the player to attack, "X" represents missed shots at the enemy. When it is time for the
enemy to attack, "*" represents missed shots at the player. 

There is logic in place to prevent the player from attacking their own ship, choosing 
an already entered coordinate either by the player or enemy, entering an invalid number 
or writing text. There is also logic that prevents the AI from choosing an invalid/already 
entered coordinate. If the player sinks the enemy ship first, they win and the program
tells the user how many tries it took for them to win. If the enemy wins then the program 
tells you how many tries it took the AI to beat you.

Once you either win or lose the program asks you if you would like to play again, where 1 = yes
and 2 = no. If you choose yes, a new game will start, if you choose no, it will thank you for 
playing and then close the program.

I added the ability for the player to choose how large the sea is, e.g. how large
the board is. The program will ask for a number (2 - 10) and whatever the player enters
a board will populate (if the player chooses 3 a 3x3 grid will be made). I think of this
as a difficult selection, where 3 is an easy/fast game and where 10 is a hard/potentially long game.
I limited the choice range from 2 to 10, just so the user couldn't enter a rediculously large number.
I also formatted any text to display the correct coordinate range to reflect the current size of the sea.

I added acception handling anytime the program asks for any user input so the program won't crash, it 
will reprompt the user to enter the correct data. This also doesn't effect any of the try counts at the
end of the program, only valid coodinate submissions are counted as tries.

Enjoy playing!
