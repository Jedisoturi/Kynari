# Kynari

A top down 1v1 turn-based tactics game. The game closely resembles a Counter Strike round in terms of goals. But instead of players controlling individual players, they control the entire team. 

## Features

* Replay: player's can view the action over and over
* Fog of war: player can only see the enemy units that are visible to his units
* Basic AI: ai characters react to enemies they see and shoot at them
* Path follow: characters follow the paths given to them by the player
* Hotseat logic: players switch only when absolutely necessary
* Bomb (this is still in an ugly state): bomb can be planted, taken from the ground, and defused.
* Own collision detection for the path drawing tool

## Detailed

The game uses a hotseat system, where the players give orders to their respective teams in turns. This is done by drawing movement paths for each soldier, and rotating them. Then both orders are executed simultaneously in the action phase. In this stage the players can view the results of their action, and repeat it as many times as they want. They can also change the replay speed. This repeats until the entire team of the other player is dead or the bomb has exploded. The hotseat logic is implemented in a way that prevents unnecessary side changes. This means that one player can usually give his orders, view the action and give additional orders before it is the other player's turn.

## Important (missing assets)

Some assets (sprites and tilemaps) are not included in this git.
