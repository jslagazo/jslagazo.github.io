---
layout: project
type: project
image: img/rpgPromptStockSquare.jpg
title: "Labor of Loyalty"
date: 2025-04-17
published: true
labels:
  - CLI
  - C++
  - GitHub
summary: "An RPG text-based beta produced by my group for our ECE 205: Object Oriented Programming course."
---

Throughout the UH Manoa ECE 205: Object Oriented Programming course, the class was pointed into the direction of completeing labs that would be based upon the previous one. This is to say that 'Lab Assignment 2' would be based on 'Lab Assignment 1' and so forth. Toward the end of the semester, the class was introduced to header files, classes, parsing, story mapping, etc. All of these concepts that were slowly integrated into our labs eventually led us to our final lab assignment for the semester which involved creating a text-based game. My group ultimately decided on making a text-based RPG called 'Labor of Loyatly.'

As far responsibility goes for this project, I was responsible for creating a story flowchart which directed the user choices all back to the same 3 possible endings for the game. Once that was established, I created the initial game character base class and later a player subclass that would inherit some game information from the base class; these were crucial as they were then followed by another subclass to allow the user to choose the specifics of their character such as name, class, and special abilities. Not only that, I also helped in creating some command-line interface for the game to make it more appealing to users. By the end of this project, I learned how important the idea of pair programming is and how this strongly correlated to the ideaa of teamwork. My group had various difficult ideas we wanted to implement, however, being able to work alongside one another opened my eyes to how differing coding styles can be better in certain applicable situations when trying to execute.

Below are two of the CLI outputs I helped develop for the game. One is of the title screen to get the game started and the other is a prompt for the user to select their next destination based on chance. Along with those is an AI generated image we established as a group for our game report's title page:

```cpp
|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
          LABOR OF LOYALTY: GAME OF THE YEAR EDITION
|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
Press any Key
```

```cpp
Imagination BGM: Scary cave ambience 
Progress: You passed through 5 doors
  ___|_|___             ___|_|___             ___|_|___
 /    1     \          /    2     \          /    3     \
|   ____    |         |   ____    |         |   ____    |
|  |    |   |         |  |    |   |         |  |    |   |
|  |    |   |         |  |    |   |         |  |    |   |
|  |____|   |         |  |____|   |         |  |____|   |
|   [==]    |         |   [==]    |         |   [==]    |
|___________|         |___________|         |___________|
You encounter three doors, one leads to a battle, another leads to a mischievous elf, and the last to an empty room. The door locks behind you when you enter. Choose wisely.
```
<img class="img-fluid" src="../img/cotton/cotton-header.png">
