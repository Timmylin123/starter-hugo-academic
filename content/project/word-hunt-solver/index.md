---
title: Word Hunt Solver
date: 2021-10-27T05:51:35.573Z
draft: false
featured: false
tags:
  - Interactive
image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
---
I constructed an interactive program with Python that can show immediate solutions to the game **Word Hunt**. 

Word Hunt is an 80-second minigame developed by [Game Pigeon](http://gamepigeonapp.com/). A player is given 16 letters on a 4x4 grid, then he will have to find out word combinations from those letters. Words can be formed in any direction but they have to be on a straight line with each letter being adjacent to the following letter in the way the word is spelled. This game is played by 2 people through text messages. The winner is the person who got the most word combo after time is passed.

I built this Word Hunt Solver on top of my previous project Anagrams Solver. In this interactive program, I utilized set theory and top-down recursion to detect all of the possible vocabulary words which can be formed in the 4x4 letter grid. A player can insert the 16 letters shown in the Word Hunt game row by row from left to right into the text bar, my interactive program would automatically show the player all of the vocabulary words that can be formed by these letters (refer to the screenshot above).

Here is my [python code](https://github.com/tinghanlin/wordhunt-solver) for my interactive program! Feel free to git clone my folder and run “*python WordHuntSolver.py”* in my folder to launch the program!