# competitive-wordle
## Project Overview
### Description
This project is a wordle clone with a matchmaking system. Each users are assigned an ELO rating, similar to chess, which allows the matchmaking system to pair players up with a similar skill level.
### Bugs / Challenges I've Encounterd
1.  Whenever users queue up, they emit multiple of the same event
    - solution: remove event emitters and listeners
2.  Coming up with an algorithm to pair users up
    - solution: decided to use a queue and pick the first user to compare its ELO rating with the rest of the players
3.  Creating user authentication without passport.js
    - solution: used JWT to access the usernames and display names
4.  Naming variables that have similar functions
5.  How to handle players refreshing page or leaving during a game
    - solution: add an event listener for sockets disconnecting
    - solution: when players refresh, it is considered as if they left and is redirected to the home page
### Features
+ User authentication
+ Skill Based Matchmaking System
+ Wordle game mechanics
+ Display player's statistics
+ Leaderboard
+ Edit username or password
+ Display opponent's progress in-game
### Screenshots
![log-in](/screenshots/log-in.png)
## Development
### Frameworks
### Tools
