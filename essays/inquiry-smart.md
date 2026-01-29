---
layout: essay
type: essay
title: "Inquiry in a 'SMART' Manner"
# All dates must be YYYY-MM-DD format!
date: 2026-01-27
published: true
labels:
  - Communication
  - Skill Development
  - Stack Overflow
---

Write a technical essay that discusses why smart questions are important for smart software engineers, how the chosen questions fulfill (or not) the precepts for smart questions, how the responses reflect the smartness (or lack thereof), and the insights you gained as a result of this experience.

Be sure that your essay includes a textual summary of both the “smart” and “not so smart” questions, as well as a link to the StackOverFlow pages where they are located. Don’t just put the URL to the questions and force the reader to visit StackOverFlow to read the question there, then switch back to your essay to continue. Your essay should contain enough detail about the two questions so that the reader doesn’t need to visit StackOverFlow to make sense of your essay.

<img width="400px" class="rounded float-start pe-4" src="../img/sqSatireCartoon.jpg">

## Why "SMART" Questions Are Enforced
As I get older, I become increasingly exposed to this idea of "*asking better formulated questions*" which sounds like a social expectation. Regardless, this expectation is really an engineering efficient rule; a prime example is its usage on websites such as [StackOverflow](https://stackoverflow.com/questions). Various communities enforce this "SMART" question approach because, answering questions come with a cost similar to formulating questions to begin with. Answering questions requires an individual's time, attention, and cognitive load. A vague question will always force helpers to reverse-engineer missing context before they can even begin diagnosing; this is wasted effort and it scales poorly when numerous people do it frequently.

In Eric Raymond's *How To Ask Questions The Smart Way*, he frames SMART questions as being able to respect the time of those who could help you. A "smart" question isn't just polite, rather it is also convenient for the helper. When the quality of the question is high, the community can produce answers that are efficient and effective. This is to say that communication requires less back-and-forth relay along with responses actually being helpful. In the perspective of StackOverflow, it represents the guidance of recreating a minimal reproducible example to reinforce the same idea shared by Eric Raymond; which is to reduce guesswork and make the issues testable. When standards like this are enforced, StackOverflow becomes a searchable knowledge base instead of a pile of barely explained problems that will never be solved.

## What Asking SMART Questions Are Like
In practice, asking a "SMART" question looks more like writing a concise report rather than typing and sending that "help pls" text to your friend about homework that is due in an hour. The core elements of this approach is consistent across languages and topics: they start with a clear one-sentence goal stating what is trying to be accomplished; they narrow down one specific failure explaining what it is and where; and they include evidence of error text or incorrect output followed by expected or actual behavior. This contrast in approach transforms the simple saying "it doesn't work" to something measurable.

Moreover, a smart question shows effort without becoming a journal entry that everyone comments "TL;DR" to. A smart approach briefly mentions what attempts were made that did not solve the issue so that helpers are prevented from repeating the same dead ends. To add, the snippet of the issue is scoped which provides enough information to reproduce the said issue without projecting an entire project dump. This why minimal reproducible examples are valued; people can run, reason, and verify issues quickly which in turn leads to confident solutions.

## Case Study of a SMART Apporach
A "SMART" example is this StackOverflow question about [TypeScript type augmentation in a monorepo library](https://stackoverflow.com/questions/79878495/how-to-add-custom-d-ts-interfaces-of-npm-module-in-a-library-and-make-it-availab). The asker gives strong context up front: they explain the setup as a monorepo with internal Typescript npm modules that are consumed by several Javascript projects and they narrow the issue down to a specific technical goal which is to extend Express's Request type with a user property. Rather than dumping their entire project into the website for everyone to look over, they provide their key evidences in what they changed and the effects it imposed.

After describing their goal, they include the exact code they wrote. The snippet makes it obvious to others what they are attempting and why Typescript would need to "see" this file during compilation.

```
// custom.d.ts
declare namespace Express {
  interface Request {
    user: RequestUserData
  }
};

interface RequestUserData {
  user_id?: number;
  user_name?: string;
};
```

They then show the **tsconfig.json** change that makes their augmentation work within the library:

```
// tsconfig.json
{
  ...
  "compilerOptions": {
    ...
    "typeRoots": ["./src/config/@types"]
  }
}
```

This is the part that makes the question "SMART,"  the individual in need does not stop at "it doesn't work." Rather, they identify the boundary of failure very clearly; the new **req.user** property is recognized inside the API module, however, it is not recognized in the projects that consume that module. That is essentially the expected versus actual behavior in plain language, it tells responders exactly what success should look like. Since the problem is tightly scoped and supported by concrete evidence, the answer can be equally as direct and useful. Instead of vague guesses, responders can explain the underlying issue and propose practical fixes. This entire exchange is the ideal "SMART" question to "SMART" help outcome I discussed earlier: minimal back-and-forth conversation, a clear root cause expressed, and a provided solution that could scale across other projects.

## Case Study of a Not so SMART Approach
A not so "SMART" example is this StackOverflow question in regards to [Word/VBA about showing and hiding a graphic via a toggle button](https://stackoverflow.com/questions/79878597/vba-command-button-action-to-display-hide-word-grahic). The asker describes what they want in broad terms and they speculate about how it might work. They mention a need for clicking a button in Word to display or hide an embedded image and if it would work via getting an object ID and setting a **Visible** property based on toggle state. The problem with this prompt is that the post never becomes an answerable debugging question since it does not provide the information responders need to work with.

Here is the question that demonstrated the lack of "SMART" structure:

```
Q: VBA command button action to display/hide word graphic

I would like to display or hide a in my word document included jpg or something based on a toggle button.
I have seen some videos about command buttons in MS Word and seems to be the way to go for me. In the action (onclick?) connected to the button
I have to put in VBA code to do the actual code. I assume this could work. First I have to include the graphic in word in some way which hopefully
gives me an (object)ID somehow which I can then use in VBA code to reference that and set a property of the object (visible?) to true or false
based on the button(toggle) value. Hope this makes sense and someone can help.

```

What is missing is exactly what Raymond and StackOverflow guidelines try to enforce. This includes no code attempt, no details about what kind of "graphic object" it is, no steps that they have attempted, and no clear expected versus actual behavior. Without these specifics, responders can't verify assumptions or test a fix; they are forced to write a broad tutorial covering possible object models and button setups. The responses reflect the responder's issue immediately; instead of providing an actual solution the first interaction is a request for missing essentials. This is a classic pattern for not "SMART" questions, helpers are forced to be inefficient and lack preciseness because the question does not provide enough evidence to diagnose anything. The topic was not an issue, rather the shape of the question being asked is.

## Creating Prompts Moving Forward
Comparing the two posts made it clear that "SMART" quesstions are not about sounding fancy, they are about reducing ambiguity so other engineers can actually help. Going forward, I want to improve in treating questions more like mini bug reports. Before asking for help, I will be sure to provide my goal clearly, the smallest step to reproduce the issue, expected and actual results, relevant environment details, and a lists of attempted fixes and how they went. If I am unable to fill in these five holes, that should be my sign that I need to work out my problem a bit more before I ask others for guidance. Asking questions this way does not just increase the chance of getting a response but, it also increases my chances of seeing a response that is correct, efficient, and applicable to other projects.
