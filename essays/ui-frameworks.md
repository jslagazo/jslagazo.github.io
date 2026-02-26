---
layout: essay
type: essay
title: "Borrowing Blueprints: Exposure to UI Frameworks"
# All dates must be YYYY-MM-DD format!
date: 2026-02-25
published: true
labels:
  - HTML
  - CSS
  - Boostrap 5
  - UI Frameworks
---

<img width="400px" class="rounded float-start pe-4" src="../img/uiFrameworksBootstrap.png">

## My First UI Framework: Another "New Language" Feeling
Prior to taking ICS 314: Software Engineering I, I had never touched a UI framework. My initial exposure to front-end work was essentially: write HTML, write CSS, refresh the page, and tweak it until it looks right. When the learning module regarding frameworks came around, it broadened my scope in understanding that CSS was not only a layout problem; it became a vocabulary problem and it gave me the idea that a "right answer" can be a combination of class names instead of an entirely new CSS rule.

An assignment I have completed in my ICS course involved recreating a simplified version of the [Island Snow](https://islandsnow.com/?srsltid=AfmBOor9a_srbCGU0A9ggV3Tyka1QLiIpPGqwkSQlaQAKNbXUN3iI9TE) web page. A great amount of the structure and alignment for this assignment happened directly in the HTML file by composing Bootstrap classes. 

<img width="400px" class="center" src="../img/uiFrameworksBootstrap"> of island snow @todo

Another assignment involved recreating a web page of our own choice; in particular, I chose a restaurant from my hometown called [Kimo's](https://www.kimosmaui.com/). The same deal applied with this assignment in that most of the composition was done through HTML via Bootstrap classes. 

<img width="400px" class="center" src="../img/uiFrameworksBootstrap"> of kimo's @todo

At first, this felt weird since I was putting 'styling' in HTML. After building a couple more web pages though, it all started to make sense. Bootstrap is not trying to replace either HTML/CSS fundamentals rather it is a form of trying to standardize the most common layout decisions so that I don't have to reinvent them every single time.

## Why Would I Bother With Bootstrap 5?
The major reason I see why many turn toward utilizing a framework is that it provides a reliable structure that prevents layout chaos. Without a framework, I can make something look correct on my screen, however, it does not protect me from the unpredictable behavior of displaying different widths when resizing the window and essential long-term code security.

Bootstrap gives me patterns that "want" to behave well. In Island Snow, I used a top navbar layout that relies on Bootstrap's navbar, nav, spacing utilities, and icon classes from [Bootstrap Icons](https://icons.getbootstrap.com/). In other words, I don't have to manually position every icon with custom CSS since Bootstrap already solves this basic alignment and spacing problem. Moreover, when creating a cart interaction I did not have to build a dropdown menu behavior from scratch. Bootstrap's dropdown structure was already there waiting for me to implement. Realistically speaking, the payoff comes to consideration when mentioning hand-building behavior and layout as opposed to plugging into a system that already expects common UI needs.

## The Return of My Investment?
As frustrating and time consuming the learning curve posed itself to be with UI Bootstrap, I ultimately benefitted in three practical ways:

1. Speed
  Once I started to familiarize myself with a few key building blocks, like **container** or **spacing utilities**, I noticed how much faster I was at building web pages. My *Island Snow* recreation is a good example of this as the layout uses multiple containers and rows to create consistent margins and spacing between sections.
2. Consistency
  Frameworks reduce "random design" and this was relevant to me as a beginner with raw CSS styling. Bootstrap pushed me toward using consistent spacing decisions and structures through use of its utilities and grid. 

  In *Island Snow*, the footer is structured as three equivalent columns using a Bootstrap row and multiple **col** elements. Doing this was cleaner than writing a custom layout approach for every instance a footer element was needed.
3. Responsiveness
  Even when I can attempt implementing responsiveness in CSS, Bootstrap's grid and responsive classes make "good enough" responsiveness easier for me especially this early on.

  In my *Kimo's* web page recreation, the info strip section is responsive using **col-md** and alignment utilities so that it is adaptable across varying screen sizes.

## So Why Not Just Use Raw HTML and CSS?
Raw

## The Software Engineering Benefits
@todo

## Where Bootstrap Still Needs "Real CSS"
@todo

## The Downsides from My Newbie Perspective
@todo

## Concluding Thoughts on UI Frameworks
@todo
