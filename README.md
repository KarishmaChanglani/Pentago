#Pentago 
##Author(s): 
- Karishma Changlani

##Discription:
A game of Pentago on the console with a built in AI (Pentago: https://en.wikipedia.org/wiki/Pentago)

##Instructions: 
Run Pentago.py with python 3.

###Board:
    1      2
    ---------------
    |1 2 3 | 1 2 3|
    |4 5 6 | 4 5 6|
    |7 8 9 | 7 8 9|
    ===============
    |1 2 3 | 1 2 3|
    |4 5 6 | 4 5 6|
    |7 8 9 | 7 8 9|
    ---------------
    3      4
  
###Move Format: 
    
    section_no/square_no section_no/rotation_direction
    
    Example if I am player b
    then my move: 3/6 1R will change the following board: 
    ---------------
    |. . w | . . .|
    |. . . | . . .|
    |. . . | . . .|
    ===============
    |. . . | . . .|
    |. . . | . . .|
    |. . . | . . .|
    ---------------
    
    To: 
    
    ---------------
    |. . . | . . .|
    |. . . | . . .|
    |. . w | . . .|
    ===============
    |. . . | . . .|
    |. . b | . . .|
    |. . . | . . .|
    ---------------
  
  
  
