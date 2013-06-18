# Chomp

1. Build a move struct with a row and column index.

2. Your board will be a R x C array of "boolean".  I will
   assume that this array is zero-based in this pseudocode.
   Initially, let R = 3, C = 4.

3. Write a function/method to initialize a board to all
   true.

4. Write a function to print a board (in ASCII, because
   graphics code takes forever). I used o and . as the board
   characters.

5. Write a function to make a move gotten from a human. Use
   whatever syntax is easy and makes you comfortable. Your
   function should return a valid Move struct. Don't overdo
   the error checking and beauty at this stage. My function
   took seven lines.

6. Write a function to make a move r, c on a board, by changing
   all squares that are at or below both r and c to false.

7. OK, here comes the interesting part...

8. Now you just need to write a main program that
   alternately calls negamax() and your human move()
   function until someone loses.
