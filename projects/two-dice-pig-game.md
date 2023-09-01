---
layout: project
type: project
image: img/pig-game.jpg
title: "Two Dice Pig Game"
date: 2021
published: true
labels:
  - Game
  - Java
summary: "For my ICS 111, I created a Two Dice Pig Game using Java"
---
For my ICS 111 assignment, I created a simulation of a Pig Dice game that uses a Graphical User Interface (GUI) in Java, in order to display an interface that displays the dice, the actions that the player can choose from, and their points. This assignment allowed me to gain a better understanding of the use of Math.random(), “while” statements, and “if” statements, which are all used to follow the rules of the game and for the program to continue running until there is a winner.

While creating this program, I have encountered many issues with the “if” statements and some compiling errors. Commenting on all of the situations that can occur for the game has helped me complete this project. This assignment has allowed me to critically evaluate the “if” statements needed in order to make this program work. 
```
      // If two 1s are rolled, the player’s entire score is lost, and the turn ends.
      if (die.rollOne == 1 && die.rollTwo == 1) {
        System.out.println("Roll Results: " + die.rollOne + ", " + die.rollTwo
            + "\nYou rolled snake eyes.\nYou loose all of your points.");
        name.setScore(0);
        turnScore = 0;
        continueTurn = false;
        
        // If a 1 is rolled, the player earns no points, and the turn ends. 
      } else if (die.rollOne == 1 || die.rollTwo == 1) {
        System.out.println("Roll Results: " + die.rollOne + ", " + die.rollTwo
            + "\nYou rolled a one.\nNo points earned.\nYour turn has ended.");
        turnScore = 0;
        continueTurn = false;
        
        // If a double is rolled, the points are added, and the user has to roll again. 
      } else if (die.rollOne == die.rollTwo) {
        turnScore += die.rollOne + die.rollTwo;
        System.out.println("Roll Results: " + die.rollOne + ", " + die.rollTwo);
        System.out.println("You earned " + (die.rollOne + die.rollTwo) + " points.");
        System.out.println("You rolled a double " + die.rollOne + "'s. You must roll again.");
        continueTurn = true;
        
        // No doubles or 1 are rolled, the points are added, and the user can choose to roll again.
      } else {
        System.out.println("Roll Results: " + die.rollOne + ", " + die.rollTwo + "\nYou earned "
            + (die.rollOne + die.rollTwo) + " points.");
```

This was one of my favorite assignments that I worked on during ICS 111, and it has motivated me to continue pursuing this major. 
