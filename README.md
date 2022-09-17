# Ballroom Blitz Wiki  
Success! You’ve infiltrated the coronation ball for the new King Azimuth in order to stage a coup and install yourself as monarch. Problem is, everyone else had roughly the same idea. Suddenly, someone in the back said “Everyone, attack!” and now it turned into a ballroom blitz! You (and everybody else it seems) figure that if you can hold the center of the room the longest, you can successfully claim the throne.  

## Contents
- [Overview and Objectives](#overview-and-objectives)  
- [The Ballroom](#the-ballroom)
- [Control Tiles](#the-control-point)
- [Endgame](#endgame)
- [Classes](#classes)
- [Items](#items)
- [Registration](#registration)

## Overview and Objectives  
Ballroom Blitz is a free for all, “King of the Hill” game. The goal is to earn as many points as possible before the game ends. Earn points through controlling the center and defeating others. There will be 4 players in a game and only one winner.

MechMania 28 will be a Swiss-system tournament.  

---

Each turn consists of four phases in the following order:
#### 1. Use Phase
Players can use any items they may be holding  
#### 2. Movement Phase
Players may do one of the following actions:
- Move to a tile
- Teleport back to the player's spawn point
#### 3. Attack Phase:
Players may do one of the following actions:
- Attack one other player of their choice who is within range
#### 4. Buy Phase:
If at their spawn point, players can choose to buy an item. As a player can only hold one item at a time, buying an item will remove any item the player was holding beforehand.   

---

- If a player is standing on their spawn point by the end of a turn, they will automatically heal for 3hp.  

- When a player’s health drops to zero, they die and respawn at their spawn point. A player will lose their currently held item upon death.

## The Ballroom 
The place you make history is the ballroom at the royal palace. The map is a square grid of 10x10 tiles. In the middle is the control point. At the four corners are the doors (spawn points) to the banquet hall.

## The Control Point 
The control point is a 2x2 set of control tiles in the middle of the ballroom. When a player ends a turn in one of the control tiles, they earn 2 points towards their score. Multiple players are allowed on the control tiles, but do you _really_ trust them?

## Endgame
Players earn points in two ways:
- 2 Points for ending a turn on the control point
- 1 Point for dealing fatal damage to another player  
   
The game ends in MAX_TURN turns. At the end of the game, the victor is decided by whomever holds the most points. If there is a tie between 2 or more players, the one who holds the most gold wins. If there is a tie in gold, the winner shall be decided by a coin flip.  

## Classes
Each class plays to a different style to dominate the Ballroom. There are 4 different stats for a class. **ALL** distances use Chebyshev distance.  
> D<sub>Chebyshev</sub> = max( |x<sub>2</sub> - x<sub>1</sub>|, |y<sub>2</sub> - y<sub>1</sub>| )
- Health: The amount of damage a player can sustain
- Damage: The amount of damage a player's attack deals, 1 damage = 1 health  
- Speed: The distance a player can move in a single turn  
- Range: The distance a player's attack can reach  

| Class  | Health | Damage | Speed | Range |  
|--------|--------|--------|-------|-------|
| Knight | 9      | 6      | 2     | 1     | 
| Wizard | 6      | 4      | 3     | 2     |  
| Archer | 3      | 2      | 4     | 3     |

## Items
Items may be purchased with gold at a player's spawn location and provides buffs and effects to assist in battle. Only one item can be held at any time. Upon dying, the player will lose any item held at the time.  
- At the end of every turn, all players automatically earn 1 gold.  

| Item                         | Attributes                                                                                                                                | Cost | Description                                                                                                                                      |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| Glass Shield                 | When used, nullifies 1 Attack on the user for 1 turn. If there are multiple Attacks in a turn, it will nullify only the single strongest. | 8G    | A sturdy glass shield said to be of Moon and Glass… Is it actually sturdy?                                                                       |
| Procrustean Iron             | Turns all Attack Damage dealt to the player equal to an attack from a Wizard while this item is held.                                     | 8G    | A corrupted fragment of iron. It forces and twists all to be the same.                                                                           |
| Rally Banner                 | Gain +2 Damage while this item is held. Cannot be used.                                                                                   | 8G    | A flag bearing what you fight for. Seeing it inspires you greatly.                                                                               |
| Anemoi Wings                 | Gain +1 Speed while this item is held. Cannot be used.                                                                                    | 8G    | A pair of wings that always seems to flutter in a soft breeze…                                                                                   |
| Hunting Scope                | Gain +1 Range while this item is held. Cannot be used.                                                                                    | 8G    | The manual claims attaching it to your weapon extends your range. You never bothered to read what type of weapon, but it probably doesn’t matter. |
| Strength Potion              | Gain +4 Damage for 1 turn.                                                                                                                | 5G    | A small vial holding a… questionable looking liquid.                                                                                             |
| Speed Potion                 | Gain +2 Speed for 1 turn.                                                                                                                 | 5G    | A flask of blue liquid. Probably safe to consume…?                                                                                               |
| Dexterity Potion             | Gain +2 Range for 1 turn.                                                                                                                 | 5G    | A bottle filled with purple liquid. Hopefully grape flavored.                                                                                    |
| Knight's Heavy Broadsword    | Allows the player to change to the Knight class                                                                                           | 10G   | Peace was never an option.                                                                                                                       |
| Wizard's Magic Staff         | Allows the player to change to the Wizard class                                                                                           | 10G   | The power of the sun in the palm(?) of your hand.                                                                                                |
| Archer's Steel-tipped Arrows | Allows the player to change to the Archer class                                                                                           | 10G   | Parry this.                                                                                                                                      |

## Registration  
For the competition, you’ll need to have the following things installed:

- Python 3. This is one of the languages you can use to implement your bot.

- Java 8. This will allow you to run the game engine locally, so you can test your code before you push it.

- [Node.js](https://nodejs.org/en/), (version 14.17.6). Once you have that installed, try running `npm i -g mechmania`. The package can be found [here](https://www.npmjs.com/package/mechmania), and when you’re able to run `mm help`, you know you'll have downloaded it correctly. From there, you can register a team by doing `mm register`. We ask that you only register once per team.

If you need help, please ask us in the Discord #ask-a-question-here channel. We'll be providing help throughout the competition!

For basic questions, please run `mm help` before asking.
