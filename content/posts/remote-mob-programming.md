+++ 
draft = true
date = 2020-03-21T08:14:05-05:00
title = "Remote Mob Programming"
description = ""
slug = "remote-mob-programming" 
tags = []
categories = []
externalLink = ""
series = []
+++

## Summary
There are many resources to read about mob programming.  There are less resources to read about remote mobbing.  I will start by sharing my learnings.  And then I will share my personal story from which my teachings have emerged.  Finally I will reveal a slightly different flavor of mobbing which I am interested in.

## My Remote Mobbing Learnings

> Use a timer and schedule your mobbing sessions in the calendar.

> Mobbing is not conducive to every software engineering situation.

> Typing speed, IDE shortcuts, and understanding terminology is an important skill for your drivers.

> A company using mob programming can hire people with the right personality who may not have any of the right knowledge of the specific technology.

> Mobbing helps to spot problems early.
[Fagner Brack](https://medium.com/@fagnerbrack/how-to-find-the-best-context-for-pair-programming-711b8fdcd259)

> Mobbing helps confer the right mindset.
[Fagner Brack](https://medium.com/@fagnerbrack/how-to-find-the-best-context-for-pair-programming-711b8fdcd259)

> The effectiveness of Mob Programming is maximized as each member of the team is multi-disciplined and capable of doing the job of anybody else.
[Fagner Brack](https://hackernoon.com/how-mob-programming-will-make-you-more-effective-590a1b7e0418)

## My Remote Mobbing Story

I started doing remote mob programming in September of 2018.  I had the privilege of working alongside 2-3 senior software engineers.  We all had about a decade of software engineering experience.  I was able to learn about the existing software at a rate that was 3x the rate it would have taken if I had been working alone.  I was also able to pick up on our overall tech stack (PHP, MySQL, and BackboneJS) at a similar rate.  This was a great experience for me as I was able to learn rapidly.  I do remember one thing that did not sit well with me at the time.  I did not like how the mob would often prioritize speed over learning.  I was more like a smart input device when I was driving.  I personally would take notes so that I could find answers at a later time without disrupting the flow.

After many months of mobbing with these excellent software engineers, my managers decided to restructure.  They made my mob members tech leads to oversee 2 mobs.  And my new mob consisted of a new hire with a similar amount of experience and a junior engineer with a couple years of total experience.  This mobbing experience was much different than my previous mobbing experience.  My new mob's productivity was not as high as the previous mob.  And my learnings changed.  I was no longer learning about the company's software with the help of people with more experience.  I was no longer learning about the technology stack with the help of people with more experience.  And I became the source of most of the ideas which were developed.

At this time I developed a web app for our mob to help with keeping track of our driving time: https://github.com/GavinPalmer1984/mobtoolbox - we used this to encourage switching drivers regularly.  My second mob did well and put out working code very rapidly.  One note from the second mob is that a mob member with limited experience can be a great driver if they know how to type fast, know how to use their IDE shortcuts, and learn the terminology being communicated by the navigator.  My recommendation is that mob members with limited experience try not to interrupt the flow while taking notes to have learnings asynchronously.  Ideally the mob member is capable of understanding complex systems and are asking the right questions in order to maintain their understanding of the complex system.  You should interrupt the flow if you have maintained an understanding and the current approach is in conflict with your understanding. 

After my second mob, I had a couple of different teams that did not really mob with much discipline.  My excuse is that I felt the team was temporary.  And new mobs can have a learning period where things move slowly before they start moving quickly.  It is also important to note that mobbing isn't really enforced at our company.  It is strongly encouraged without much oversight.  Its being enforced depends on the tech lead responsible for overseeing the mobs.  I personally have a more disciplined approach when someone voices a desire to do strict mobbing.  It is in those moments when I enjoy revealing my mobtoolbox web app.

I eventually found myself in a solid 3rd mob composed of two people that brought knowledge to the mob which I lacked.  I find that I really enjoy mobbing with people who bring a lot of useful knowledge to the team.  One mob member voiced interest in strict mobbing and so I revealed the mobtoolbox and we scheduled our daily mobbing sessions in the calendar.  I think we might have had the most productive backend mob at our company at that point in time.  I got to learn more about php and software design in general.  I am good at reading code.  But I am not the best at writing the cleanest code.  And so this mob helped me get better at recognizing and writing cleaner code.

The senior software engineer with similar years of experience as my own in the 3rd mob was moved out and an entry level software developer was brought in.  He did not work out and he was swapped with another entry level software developer.  This last month or so is my first experience mobbing as a senior software engineer without any other senior software engineer.  And I have an entry level software developer as well.  I like the people in my mob.  But I think this is the least productive mob composition I have experienced.

## Directed Pair Programming

What is the value of adding an entry level software developer to the mob?  When they are driving they are moving slowly.  They don't understand the terminology.  And they can't learn the terminology as fast as someone who has already become proficient at a programming language.  They haven't learned the IDE shortcuts.  And they may even be slow typers.  When they are not driving they may occasionally spot a typo.  But if that is really adding value to the mob then it means your other mob members aren't really paying attention.

Entry level software developers in a mob can add value by understanding the user stories which are being addressed and helping to verify that everything is working as expected.  They should learn to type fast, use IDE shortcuts, and try to understand the terminology being used by the navigator.  They should take notes and avoid interrupting the flow.

One thing I like about this composition of having an entry level software developer in a remote mob is that you can only ever have one driver and one navigator.  The other people in the mob really shouldn't be talking too much once development begins after design has taken place.  Because the entry level software developer has so little understanding of the language being used, the navigator has to be very explicit in their communication.  As the non-driver and non-navigator, I am able to follow along without my eyes.  I am able to listen to the software development.  And this is amazing in my opinion!  With practice I could listen to more than one of these guided remote pair coders simultaenously!  This is the ultimate smart input device for an experienced software engineer.

I get to ask the important questions about the design.  I get to create visualtions for the design if it is needed.  I then get to listen to the development of those designs and review them in real time.

The goal of a technical manager of software engineering at every level is to encourage your team members to be able to do the work on their own without you while helping them to become capable of taking on the role you are currently performing.