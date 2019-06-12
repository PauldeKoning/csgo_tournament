CSGO TOURNAMENT
===============

csgo_tournament is a repository for a Counter Strike Tournament system. 

It includes a database, a csgo server plugin and a small front-end.

### Database

The database is quite small, it has the basics needed to store a game, players, teams, team invites, map veto and give information to the server about who joined.

### CSGO server plugin

The main part of this repository is the csgo server plugin. Currenly it is possible to play an entire game with this plugin and a chosen config file.

It connects to the database where it requests what game is currently playing for the joined user. If there is a game playing for this user, it lets him join.

When the player joins he can join any team. The moment he types .ready, he ready ups and when everyone is ready, the game will switch everyone to their starting sides and start the game.

The players can type .timeout to start a timeout which they have four of.

When the game ends, all players get kicked off, data of the game (can) get sent to the database such as leaderboards. After players are kicked the server goes to idle mode and it waits for new players.

### Front end

The front end is a small website that can display the games, teams and players. You can invite people to your team, change your team logo and change your player name. You connect your account via the steam API.