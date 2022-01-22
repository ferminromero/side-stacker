### TODO

 - Create 7x7 grid UI in React app
	- Hooks - UseState, UseEffect
- write postgres data model
	- store each move in a table: player, row, side, timestamp, game number
- connect node server to db
- implement function to start a new game
- implement function to add a new move to the database
- implement function to check the current game for a winner
- Figure out websockets
	- Handshake
	- Send message from server to client
		- Game started
		- A player has won
		- Disconnect
	- Send messages from client to server: Move made, Disconnect
	- Only 2 players in game - how are they assigned unique IDs?
	- If game is in progress, reject incoming connections (only 1 game at a time)




## Notes: 
- each time a move is made, run a function to check the board for the winning condition. because this is run each time a move is made, we only have to check for a win condition starting with the coordinate of the new piece.
- For database, store a log of moves?


## DB Schema
table: turns
game number, player, row, timestamp
	- player, row, left/right




- board is like this:
0 [ _ _ _ _ _ _ _ ]

1 [ o x _ _ _ _ o ]

2 [ x _ _ _ _ _ x ]

3 [ x _ _ _ _ _ o ]

4 [ o _ _ _ _ _ _ ]

5 [ _ _ _ _ _ _ _ ]

6 [ _ _ _ _ _ _ _ ]
