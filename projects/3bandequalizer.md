---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "3-Band Analog Equalizer"
date: 2025-12-08
published: true
labels:
  - MATLAB
  - LTSpice
  - Circuit Simulation
summary: "In UH Manoa's ECE 326: Microelectronics II course, my team based our final project on desinging a 3-band analog equalizer for vehicles utilzing transistors instead of common BJTs."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

Microelectronics is imperative to society in various ways. Reponsible for essential data functioning and the existence of modern devices, this final project in UH Manoa's ECE 326: Microelectronics II course curriculum encapsulates all that the student has learned in both prior and current course to exhibit a device or system that is important to thriving communities today. To begin, students form groups or work independently to discuss and choose a relevant need/commodity. Following this, students were tasked in investigating their chosen topic and establishing a motivation for pursuing the application. Lastly, students are challenged with implementing their topic, developing an engineering-based analysis, and sharing their findings to the class via techinal presentation and IEEE report.

For this final project, I was responsible for assembling the presentations that were shared in class, proposing circuit schematic implementations to help with debugging and sanity checks, as well as writing the abstract and conclusion for the written IEEE report. I began by first discussing with my group our goals in designing an equalizer. Our varying backgrounds living in the state of Hawai'i were all interconnectted solely by our inspiration, preference, and vulnerability for the sound system displays of Hawai'i. I developed and assembled presentations to our topic by going into depth with the relevance equalizers held in car audio systems; introducing the specifics to why audio systems sound the way they do and how they are fine tuned to reach focused specifications. When our group was finished with our initial design schematics, I took initiative in plugging values into the circuit and making measurements that aligned realistically with those concepts learned in class. After sharing all of our findings with our peers, I helped summarize, reinstate, and finalize the written report we developed in accordance to our final product.

Here is a snippet of the schematic we developed for this project:

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

If you are interested in learning more about this project, our written report can be found [here](https://docs.google.com/document/d/1sgpkPRnQSQnF0SSexefx18nQnNjKp4HZeSLet5IbBq0/edit?usp=sharing).
