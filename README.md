# Boggle

## To Run
Download zip, navigate to the directory the zip file is in and run "java -jar Boggle.jar" in the terminal. 

## Background 
Generally speaking, Boggle is a board game where you are given a certain grid of letters and you are tasked with finding as many valid words as possible in a certain amount of time. Ordinarily, you would be able to compete with fellow human minds. However, this java implementation of this popular word game allows you to challenge yourself and go head to head with the computer!

## Features 
This particular implementation allows the user to choose the size of the board they play on. Players can choose to play the original Boggle (4x4 grid), Big Boggle (5x5 grid) or Super Boggle (6x6 grid). The user also has the option to play a bonus version of each game, which has ‘bonus’ tiles in each row of the grid worth extra points. At the end of the game, an algorithm will generate all possible words that the user could have guessed from that particular Boggle grid.

The player will have 90 seconds to find as many valid words as they can, along with the option to end the game earlier by clicking on the “Finished early?” button. If the player is stuck, the “Hint” button displays the first two letters of a possible word and deducts two points from the score. A word can be formed by clicking on the tiles in order and then clicking on the “Found Word” button, which checks for validity and updates the score. The word must be a valid word (meaning that it can be found in a dictionary), each character in it has to be adjacent to the next and the word itself must have at least 3 letters. Given the immense size of dictionaries, checking to see if the word exists in a dictionary can be tricky.

This implementation makes use of a Trie to store the words in the dictionary. A Trie is a specialized data structure that requires more memory than trees and lists. However, in specific cases (such as this one), it is effective in improving performance. This particular implementation uses a Trie to store these words because it has relatively quick lookup in comparison to other data structures.
