---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Two Dice Pig Game"
date: 2021
published: true
labels:
  - Game
  - Java
summary: "For my ICS 111, I created a Two Dice Pig Game using Java"
---
For my ICS 111 assignment, I created a simulation of a Pig Dice game using Java. The program asks the user for the amount of players that are playing and asks for their name. When it's a player’s turn, then they must roll the dice. If they roll a one on their dice, then they don't earn any points. If they roll one’s on both of the dice, then the player loses all of their points. If the player does not roll any one’s then they earn points and can choose to roll again. The first player to 100 points wins the game. 

While creating this program, I have encountered many issues with the “if” statements and some compiling errors. Commenting on all of the situations that can occur for the game has helped me complete this project. This assignment has allowed me to critically evaluate the “if” statements needed in order to make this program work. 

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```
