---
layout: essay
type: essay
title: "Coding Standards: Inevitable Red Squiggles"
# All dates must be YYYY-MM-DD format!
date: 2026-02-11
published: true
labels:
  - Coding Standards
  - ESLint
  - Visual Studio Code
---

<img width="400px" class="rounded float-start pe-4" src="../img/csSatireCartoon.png">

## Coding Standards Are Not for "Style"
Prior to entering the 'QA Part 1: Coding standards' module in my ICS 314: Software Engineering I course, I thought coding standards mainly resided in the area of neat yet petty coding. That is to say, it was only applicable to minor issues such as the difference in uses between tabs and spaces, the location of braces, and the placement of semicolons. After about a week of using the ESLint extension in Virtual Studio Code, I would be lying if I said I still saw coding standards in that same notion. Looking at it now, coding standards feel less like decorative implementations and more like guardrails. 

The standards help maintain and keep me from drifting into writing code that "works like a champ" today but, has to be taken "out back like Old Yeller" the next day for its painful environment in reading, debugging, or code expansion. Speaking on expansion, what surprised me the most about coding standards is not its capability in protecting others from my code rather its strength in also protecting future me. It's a given there will always be version of me who comes back days and even weeks later to a previously written code and ask myself "What made me choose to do it this way?" When standards become consistent, the code itself undeniably answers that question faster than trying to think for a reason myself.

## The Underlying Costs of "If It Ain't Broke, Don't Fix It"
In almost every project an individual creates, the ease in treating their matching output to the given expected result as the finish line for a coding task is often tempting. For me, I find myself thinking this way while I attempt some of the practice WODs (Workout of The Day) for my ICS 314 course as I am juggling between 5 other courses this Spring semester. I did notice though that exposure to ESLint helped in pushing this type of mindset back. I noticed myself picking up emphasis on the idea that software is not only about correctness but, its also about clarity, consistency, and maintainability. 

For instance, warning messages about unused variables or wrong implementation of logic are not just "noise." The "noise" often points to crucial considerations, two of the most common considerations I have been getting with my lint errors revolve around:

1. Implementing an idea and abandoning it, leading to compiler confusion
2. Misunderstanding my code path and accidentally writing code that never matters

In either case, the lint errors forces me to remove abandoned clutter and justify the design I intend on portraying through my code. That being said, it helps me reduce my code's ambiguity which I feel is important to spotting bugs.

## ESLint as a Teacher?
A claim I did not really believe in at first is that coding standards can help enforce learning a programming language. After working with ESLint in VS Code, I completely understand why people wholeheartedly support this. Lint rules don't just tell you something in your code is wrong. Instead, lint rules imply why your code is risky and over time more patterns start to show: consistent naming makes it easier to reason about types and intent; rules about equality, variables, and unreachable conditions reduce logical errors; encouragement toward coherent control flow makes code easier to test. In all honesty, I think of ESLint as having a strict reviewer sitting next to me. The reviewer does not have the intent of shaming me but, they enforce habits on me that keeps impracticality from growing.

## Are Coding Standards More Harm Than Good?
Through my experiences so far in attempting to get rid of lint errors, I found them very annoying. This applies especially in cases where I feel confident that my code is fine as is since it works. I was not aware that there existed a type of frustration when you become deep into problem-solving mode and a tool is there waiting at the end to interrupt you over a formatting detail.

Although I get frustrated dealing with lint errors, I get a feeling of satisfaction once I resolve the issues. The irritating task of going through the lint errors is often front-loaded and the useful takeaway of linting is its long term payoff. These payoffs could be things such as fewer confusing states, fewer mystery variables, fewer disrupted edge case behaviors, and just overall more consistent structure establishment. As the lint rules become more of a habit, I expect less fighting against it and more of a better yield in first draft creations.

## Coding Standards in Panoptic View
A valuable shift in my perspective to coding standards is realizing that these standards act as a form of communication. Code is not just instructions for the computer but, it is also a message to the next person reading it. Resolving lint errors made me reminisce about a past project I have worked on that enforced pair programming. When everyone follows the same convention, everyone gets to spend less time decoding the style; they can allocate more time toward understanding the logic itself. Although I may be working alone, ESLint can simulate a team environment to me by holding myself accountable to a consistent baseline.

On another note, I could see why coding standards are vulnerable to getting a bad reputation in that it sounds like it restricts creativity. I believe otherwise in that good coding standards do not remove creativity in problem-solving and instead removes pointless decision making. If I don't need to spend time thinking about formatting or naming consistency, I surely can spend it where it matters like designing data structure, choosing an algorithm, and writing out test cases. Coding standards can essentially present itself as a paradox; where the constraints increase productivity by minimizing the range of mistakes.

## Approach to Coding Standards Moving Forward
Following through with my experiences in the future, I do not want to make it a goal to completely get so good at writing code that it never triggers the ESLint extension in VS Code. My goal is to write code where I can anticipate lint errors to the extent that they rarely surprise as opposed to how they do now. I think my default habits align closely in practice, yet maintaining the practice accordingly is my goal. Coding standards are not trivial, they are responsible for shaping how one thinks while they code. So if I had to choose one technique to improve my overall software quality, I would follow exactly as to what was expressed in my ICS 314 course in that coding standards is the number one priority.
