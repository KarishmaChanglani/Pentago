Pentago
Functions: 
rotate: 
	Rotates a block of the grid
Params: 
	@grid: the current grid
	@move: the rotation move
Return:
	grid after rotation
	copyGrid: 
		shallow copies a grid into a new variable without mutation the original grid
		Params:
			@grid: the grid to be copied
		Return:
			newgrid: the grid copied
	makeMove: 
		Adds the intended piece to the grid
		Params:
			@grid: the current grid
			@color: the player color
			@moveL the drop move
		Return:
			Grid after drop move
	checkWin: 
		Checks if the move leads to a win condition:
		Params: 
			@grid: the current grid
		Returns:
			The winning condition if one exists else None
	checkWinColor: 
		Checks win condition for each color for the sake of simplicity. 
		params: 
			@color: the color to be checked
			@grid: the current grid
		return:
			win: win condition for the color in boolean
genRandomMove: 
		Generates move for the computer randomly (player 2)
		Params: 
			@grid: the current grid
		Returns: 
			A random move that is valid
	genMinMax: 
		Generates move base on min max algorithm and executes alpha beta pruning:
		Params: 	
			@grid: Grid of the game
			@playerno: the player value to determine the color piece for the computer
			@moves: the current streak of moves
			@depth: the depth bound for min max
			@alpha: the alpha for pruning
			@beta: the beta for pruning
			@maximizing: to check if we are in max or min state
		Returns
bestScoreAndMove: a tuple that contains the best score and the best move for recursive purposes. 
allPossibleMoves: 
	Params:
		@grid: The current grid state
	Returns:
		moves: a list of all possible valid moves in the grid. 
	
Pentago:
	Runs the game for the two players till there is a winner.
	Calls all the previous stated functions.
	Params: 
		@grid: the previous grid
		@p1: the player 1 name
		@p2: the player 2 name
		@userplayer: the choice of player the user wants to be
Problems:
	There are currently a lot of problems with the code. Mainly it’s broken functionality of min max when ran with the game. The min max algorithm works alone with alpha beta pruning. The random algorithm still works.
