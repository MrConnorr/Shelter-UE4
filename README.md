# Shelter

## Game Description

A video game version of tabletop game "Shelter". You are given an Apocalyptic descritption (e.x. Zombie Apocalypse), then you are given a Shelter Description, like how many people can stay there, for how long, what size of Shelter you have, is there any medical bay etc. Then each player getting unique stats like they occupation, their traits, health status, inventory etc. and each player getting 2 Ace Cards for example "Knows the location of supply store". Ace cards unique, so there are no duplicates. Then, each round every playes reveals one of their stats and can use their ace card (1 per round). Then, for example, each 2 rounds you need to kick one player out by voting and you need keep kicking players until there are enough space in Shelter. So for example, you are group of 6 players, you need to kick 3 players to finish the game. For eveyr player goal is the same, to get into the shelter but there is a catch, since every stats is randomized you can be a doctor with perfect health but you could be claustrophobic, you need to hide it to get into Shelter or else you lost.

## Installation

### Android

Simply, install apk the way that are most suitable for you.

### Windows

Just run exe file from game folder

##### Note! Since game was developed mostly for mobile devices, UI may look weird in fullscreen, just press ALT+Enter and resieze it as you want.


## Server Running

From the server folder, run "Start Shelter Server" that way you will get log of the server.
Before runnig the server, you need to set up NAT Forwarding in your router settings. Basically, opening 7777 port for the server. That way, users will be able to connect to it despite their location.

## Connecting to Server

1. Open the game
2. Choose your username
3. Enter IP address of the server. It is IP address of the person who is running server, you can find your IP address just by Google "What's my IP".
4. Enjoy!

## Server console commands

You can open console by pressing: If on Android, 4 fingers on the screen, If on Windows, by pressing "`" on your keyboard. ![key-button](https://user-images.githubusercontent.com/33956083/155344734-9d62f819-8d01-4038-bca7-cbe6f0ec9e8c.png)

- open L_levelName - Will open selected level
  Existing levels:
  - L_MainMenu
  - L_Lobby
  - L_MainGame
- ce ChangeSettings [Int:MaxNumOfPlayers] - will change maximum number of players. Note! If players less or more than maximum number, players wont be able to press "Ready" button and therefore wont be able to start a game.
- ce SetupPlayer [Int:PlayerId] [Bool:isNewPlayer] - will setup player with new random stats or if the player connected after the game started, you can setup him with new stats and set him with Apocalypse and Shelter description that already were generated. (So, no need to restart the game).
- ce SetupGame - will randomize new Apocalypse, Shelter and stats for all players.


## Troubleshooting

Most troubleshooting comes just with restarting the server, but if there are any probles with UI or player side, just make an issue and I will look into it.
