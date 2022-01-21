Currents - Take Home Project


Frontend - React hooks
 UseState
 UseEffect

To Do
- write data model for 7x7 grid
- create schema, initialize db and connect it to node server


Store a list of moves?
- list of moves:
	- player, row, left/right



- each time a move is made, run a function to check the board for the winning condition.
- because this is run each time a move is made, we only have to check for a win condition starting with the coordinate of the new piece.



- board is like this:
0 [ _ _ _ _ _ _ _ ]

1 [ o x _ _ _ _ o ]

2 [ x _ _ _ _ _ x ]

3 [ x _ _ _ _ _ o ]

4 [ o _ _ _ _ _ _ ]

5 [ _ _ _ _ _ _ _ ]

6 [ _ _ _ _ _ _ _ ]


- create nodejs server
- connect node server to postgres db
- figure out how to communicate over websockets

- create frontend react app
- websockets again
