# Partygame
NOTE: All videos are currently not recorded in fullscreen. This makes the video look a bit "off", as a part of the game is not recorded.
# What is this?
"Party Game" is a game were the participants use their smartphone as a controller to play different minigames. The idea is that you run a game on a computer, and each player connects to the game through an app or a localhost webpage(Not supported yet).

The game contains multiple small minigames, with a game length that vary from 20 seconds up to 10-20 minutes.

# Requirements
To play the game, you will need the following:
* A computer, capable of running java 
* For each participant, an ios or an android smartphone or tablet
* A wifi router or a computer simulating a wifi router
  * Newer windows laptops may have this feature
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

# Implemented features

## Split screen
Watch a demo of split screen

[![Split screen demo](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/vnz3e)

Demo of splitscreen.

## Screen shake
Click the picture to watch a demo of screen shake

[![Screen shake demo](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/xgzb3)

Demo of screen shake.

# Minigames
As of now, the game consists of 5 minigames.

## Count the number
Click on the picture to watch a demo of the minigame

[![Count the number video](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/c65zt)

This minigame is about counting the number of entities passing through the screen. The winner is the player that counted the nearest amount.

The controller for this game is a simple button, and for each button press, the player has counted an entity. If the players presses the button 10 times throughout the minigame, the player counted a total of 10 entities.

## Achtung 
Click on the picture to watch a demo of the minigame

[![Achtung video](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/k14ji)

This minigame is a remake of the old game Achtung die kurve. In this minigame you control a snake, and the goal is to be the last survivor. If you hit the edges of the screen or another player, you die.

The controller for this game is two buttons, one steering the snake to the left and the other to the right.

## Maze game
Click on the picture to watch a demo of the minigame

[![Maze video](https://raw.githubusercontent.com/joakimandal/Partygame/master/countthenumber.png)](https://streamable.com/ri98f)

This minigame is about controlling a box and maneuvering this box through a maze. If you hit a wall in the maze, your position will be reset back to the starting position. The goal of this minigame is to reach the goal first.

The controller of this minigame is simulating a touchpad on a laptop. The player touches the screen with a finger, and "moves" the box on the screen. Ex. dragging the finger left will move the box to the left.

## Platformer speedrun
This minigame is about controller an entity and maneuvering this entity through a map like a platformer. You can move left and right, and jump if you are standing on ground or sliding down a wall(Wall jump). The goal of this game is to reach the goal first.

The controller of this minigame is a joystick and a button. The joystick is used to go either left or right, and the button is used to jump. 

## Top down shooter
Click on the picture to watch a demo of the minigame


