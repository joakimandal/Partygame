# Partygame
NOTE:
* Some of the videos are currently not recorded in fullscreen. This makes the video look a bit "off", as a part of the game window is not recorded.
* All assets are currently placeholder assets and will most likely be replaced in the future.
* All UI are temporary and will most likely be replaced in the future.

# What is this?
"Party Game" is a game were the participants use their smartphone as a controller to play different minigames. The idea is that you run a game on a computer, and each player connects to the game through an app or a localhost webpage(Not supported yet).

The game contains multiple small minigames, with a game length that vary from 20 seconds up to 10-20 minutes.

# Requirements
To play the game, you will need the following:
* A computer, capable of running java 
* For each participant, an ios or an android smartphone or tablet
* A wifi router or a local hotspot
  * Newer windows' laptops may have this hotspot feature
  * Most smartphones have this hotspot feature
  * There is no need for an internet connection. All you need is to connect the computer and phone through local wifi.

  
# Pictures of client controllers
When launching the app, the app shows a connect button so that the player can connect to the game.


![Connect](https://raw.githubusercontent.com/joakimandal/Partygame/master/connect.png)

Clicking the connect button will show an input dialog where you write a name that will be shown on the game(running on the computer).

After writing a name and connecting, the first player will get a "leader controller", so that he can change settings and start a game. 

![Leader controller](https://raw.githubusercontent.com/joakimandal/Partygame/master/leadercontroller.png)

The rest of the players will get a screen showing that they are connected, and waiting for the leader to start a game.

![Connected, not leader](https://raw.githubusercontent.com/joakimandal/Partygame/master/conntectedtwo.png)

When all players are connected, the leader can choose a minigame. When a minigame is selected, the game will send a controller to all players. This controller will now send input to the server.

# Minigames
As of now, the game consists of 5 minigames.

## Count the number
Click on the picture to watch a demo of the minigame

[![Count the number video](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/c65zt)

This minigame is about counting the number of entities passing through the screen. The winner is the player that counted the nearest amount.

The controller for this game is a simple button, and for each button press, the player has counted an entity. If the player presses the button 10 times throughout the minigame, the player counted a total of 10 entities.

## Achtung 
Click on the picture to watch a demo of the minigame

[![Achtung video](https://raw.githubusercontent.com/joakimandal/Partygame/master/achtung.png)](https://streamable.com/k14ji)

This minigame is a remake of the old game Achtung die kurve. In this minigame you control a snake, and the goal is to be the last survivor. If you hit the edges of the screen or another player, you die.

The controller for this game is two buttons, one steering the snake to the left and the other to the right.

## Maze game
Click on the picture to watch a demo of the minigame

[![Maze video](https://raw.githubusercontent.com/joakimandal/Partygame/master/maze.png)](https://streamable.com/ri98f)

This minigame is about controlling a box and maneuvering this box through a maze. If you hit a wall in the maze, your position will be reset back to the starting position. The goal of this minigame is to reach the goal first.

The controller of this minigame is simulating a touchpad on a laptop. The player touches the screen with a finger, and "moves" the box on the screen. Ex. dragging the finger left will move the box to the left.

## Platformer speedrun
This minigame is about controlling an entity and maneuvering this entity through a map like a platformer. You can move left and right, and jump if you are standing on ground or sliding down a wall(Wall jump). The goal of this game is to reach the goal first.

The controller of this minigame is a joystick and a button. The joystick is used to go either left or right, and the button is used to jump. 

## Top down shooter
This minigame is a top-down minigame where each player controls an entity. At the start of the game, each player chooses a set of "spells" or "attacks". Some of these spells are defensive, while other are offensive. Most offensive spells will deal damage to other players on hit, reducing their health. When your health is 0 or below, you are dead. The goal of this game is to be the last survivor.

The controller of this minigame is a joystick and 3 buttons. The joystick are used to move the player entity, and the buttons are pressed to use the spells chosen at the start of the game. Ex button 1 will use chosen spell 1, button 2 will use chosen spell 2. ect. 

Each spell has a given cooldown, and can only be used if the spell is not on cooldown.


# Implemented features

## Split screen
Watch a demo of split screen

[![Split screen demo](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/vnz3e)

Demo of splitscreen. There are currently not any max number of players when using the split screen mode, but if the player size is larger than 8 players, each split screen area would most likely become too small.

## Screen shake
Click the picture to watch a demo of screen shake

[![Screen shake demo](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/xgzb3)

Demo of screen shake. In this demo, screen shake is applied when a player entity hits the ground. The screen shake applied is based on the y-velocity of the player. 


# FAQ

What language is this game written in?
* The game is written in Java, using the framework Libgdx. The framework Kryonet is used for networking.


Which controller input types are supported?

The game currently supports the following input types:
* Buttons. Sends button down and button up events to the server.
* Joystick. Sends continous input when the joystick is touched.
* Touchpad. The touchpad simulates a laptop touchpad, sending touch drags to the server.
* Accelerometer. The accelerometer sends continous input about how you hold your phone. 
