# SpaceInvaders
My version of the famous game "SpaceInvaders" using my game engine.
* The best way to showcase the game engine and its features is by building *my versions* of the famous game ***SpaceInvaders***

![alt text](https://github.com/ssudher/SpaceInvaders/blob/main/SpaceInvaders/SpaceInvaders.png)

## You want to try that game yourself?
* Just download this repository - [SpaceInvaders](https://github.com/ssudher/SpaceInvaders)
* Download the entire repo and then Click on the **SpaceInvaders.exe** in the folder and start playing

## Rules, features, gameplay and controls:
*'A' - Move left, 'D' - Move right, 'Spacebar' - shoot laser*
* The user’s spaceship is the textured yellow ball, and it is controlled using ‘A’ and ‘D’ to move left or right.
* The enemy spaceships (light-blue textured rectangles) will move from side to side and also gradually move downwards. It is a subtle movement that is evident when you play.
* The enemy ships fire towards the user’s ship randomly after a few game loop iterations. When you collide with this orange bullet you lose the game.
* The user’s shape-ship can also fire using the ‘spacebar’. The user’s firepower is restricted to 3 at a time. When you hit the enemy target correctly, you effectively destroy that ship. Inorder to win you must destroy all the ships before they reach the critical zone marked in red (***deathzone***).
* There are some features like speed up or slow down the user’s spaceship. This can make the game easier or difficult. Use the ‘UP’ and ‘DOWN’ arrow keys to control the speed.
* I have also given a ***‘GODMODE’*** by pressing the key **‘G’**. While in godmode, the user can fire as much as 100 bullets at a time and will not die due to enemy’s firepower. But you will still lose the game when the enemy spaceship reaches the deathzone.

## What's under the hood?
* The enemy spaceship movements are raised as an event and handled in the script at every loop
* The user’s space-ship can move faster or slower based on keyboard inputs. (UP and DOWN arrows) making use of the timeline.
* The enemy spaceship and the user’s spaceship both shoot bullets/laser whatever you want it to be, which essentially is just a moving platform. This uses the game object models to make it possible to spawn and destroy objects with ease.
* Once these bullets are fired from either side, it needs to trigger other events like death which uses the collision detection and handling system in the game engine.
* I have built this game to be primarily a single player game, but the game-engine has support for multiplayer architecture as well.

***Interested in knowing how the game-engine is designed?, take a look "under" the hood of [my game engine](https://github.com/ssudher/CSC591)***
