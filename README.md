# Introduction
Simple tool that will help you on manage your statistics in League of legends live games.

## How does it work?

YourLOLassistant interacts via HTTPS Requests on official League of Legends API.
The live game data is received via the League Client API that  provides a method for gathering data during an active game. It works only locally on port 2999.

## yourLOLassistant

The use of the application is summarized in two interfaces: hub and live game.
- Hub: Show game data information about a single player. Such as the player rank and his winrate ratio or the last 20 games played from him with his statistics.
  + ![alt text](https://github.com/UniCT-WebDevelopment/YourLOLassistant/blob/main/docs/hub.png)
- Game: Show the live game data, which helps the player to monitorize his statistics.
  + ![alt text](https://github.com/UniCT-WebDevelopment/YourLOLassistant/blob/main/docs/match-tab.png)
 + ![alt text](https://github.com/UniCT-WebDevelopment/YourLOLassistant/blob/main/docs/stats.png)
## Features

- YourLOLassistant detects when the game starts and take you to the live game interface. 
- In live game interface you can choose which statistics you want to show or not, and give you the chance to rollback your choise.
- In live game interface you are able to "click" on a champion inside the match table menu, allowing to look at the information about the player.


## Prerequisites

- Install [NodeJS](https://nodejs.org/en/). I recommend that you use the latest LTS version available.
- Install Electron: 
  + ``` npm install --save-dev electron ``` 
## Run

Starting out the application is really easy. First of all, clone the project repository:

- Cloning and change directory:
  + ```$ git clone https://github.com/iByrs/yourLOLassistant.git ```
  + ```$ cd yourLOLassistant```
- Build your app
  + ``` $ npm run make``` 
- ENJOY!

## Note to read before running the application:
There are small steps you must do before running the application,
The League of Legends client and the game client use a self-signed certificate for HTTPS requests. To use the Game Client API, you can ignore these errors or use the [root certificate](https://static.developer.riotgames.com/docs/lol/riotgames.pem) to validate the game client's SSL certificate.

# Note
YourLOLassistant is a university project made by student Vincent Pastor (X81000834) from the University of Catania for the subject Web Programming 20/21.
