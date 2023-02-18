---
title: "AWS re:Invent 2022 - CodeWhisperer"
date: 2023-02-05T09:00:00+10:00
draft: false
tags: ["aws", "ml", "amazon-web-services"]
cover:
    image: "posts/reinvent-2022-codewhisperer/images/1.png"
    caption: "So AI is just my writing code for me now?"
    relative: true
---

# You’ve watched the live streams in previous years, now it’s time to attend the live event!
I was lucky enough last year to attend the one and only re:Invent for the first time - after watching many online I was pumped to get my feet on the ground in Vegas and start learning, for better or worse!

# Builder Sessions - Where you’ll find me
At re:Invent there’s thousands of sessions, which fall under particular categories - one in particular that had me hooked - Builders’ Sessions!
There’s nothing like getting your hands dirty when you’re trying to learn a new technology and re:Invent gave me the opportunity to do this in stellar fashion.

During re:Invent the team members that work on the services you’ll be building within often run the session themselves, so not only do you have the best teachers around just a question away, you’ve also got the most enthusiastic teachers around - the passion shown during many of the sessions was undeniable.

I was lucky (and crazy) enough to secure a number of Builders’ Session as soon as they were released at 4AM - with one of the sessions I secured being today’s topic - AIM325, named “Build applications faster with an ML-powered coding companion”.

# So AI is just my writing code for me now?
Unfortunately, the short answer is; no. _Companion_ is the key word here. 
You will still have a job - no worries there, also unfortunately, some might say.

[Amazon CodeWhisperer](https://aws.amazon.com/codewhisperer/) is sold as “… a machine learning (ML)–powered service that helps improve developer productivity by generating code recommendations based on their comments in natural language and code in the integrated development environment (IDE).” which, whilst sounding innocent enough, sounds almost too good.
Based on my comments it’ll just _know_ what I’m trying to do?

I have seen this technology being greeted with mixed responses - which is understandable, given the nature of the service. 
Understanding and owning the source code you’re implementing is not a process not to be taken lightly - we’ve all been guilty of the StackOverflow copy-paste saga where you copy code, believing it’ll solve all your problems but instead up end up going down a rabbit hole that ultimately brings you no closer to goal of solving _your_ problem.

# From Comments to Code
Our first task was set - download an image file and upload this file content to an S3 bucket - sounds rudimentary enough, and a perfect candidate for CodeWhisperer. 
Why reinvent the wheel when you have your coding companion to help fill in the blanks?

Your companion needs input though - it’s not a mind reader (yet) so the team had some provided attendees prompts to help us get started;

> \# Function to get a file from url

With our comment in place, ready for interpretation we hit the enter button and CodeWhisperer swings into action.
Going through what CodeWhisperer returned, I received two different implementations that looked viable, and the rest which I either disregarded as too complex or just invalid - which is the first point where you, the developer, have to think.
Which implementation actually does what I want, and returns what I want!

Next up was the next step - uploading the contents to an S3 bucket.

> \# Function to upload image to S3  

Sound easy enough right?
The key to this lies in what we chose previously though - we need a function that will accept what the previous function returns.
Unfortunately I wasn’t switched on and in this second stage chose a solution CodeWhisperer returned that didn’t accept what my first step was returning - which is the second point, the developer, have to think, again!
Are these suggestions CodeWhisperer compatible with my existing implementation?

I ended up having to go back a few times throughout the sessions to change implementation details, by either re-invoking CodeWhisperer to go through alternative implementations or taking things into my own hands and changing the details myself.

# So you’re what saying is… I still have to think!
Yes - you’re still in control and need to understand what’s going to to be able to make the final decisions around what’s being implemented - which is a good thing, as you’ll be ultimately responsible once that code has gone into production use!

What this session proved to me was that **CodeWhisperer has the ability to help get the get the creative juices flowing** - through suggesting implementations for routine operations I was able to get through these low-value steps faster, which if and when I’m doing these routines operations as a part of a bigger project would help me move towards implementing the difficult - and more valuable - business logic, rather than spend my time looking up that previous implementation of an S3 bucket uploader, for example.

# Final Verdict - It’s got my vote 👍
Over the Christmas holidays I retried this Builders’ Session, spending more time going through what CodeWhisperer was returning and playing with the results - what happens when I change the prompt slightly, what happens when I’m trying to forcibly direct it towards a particular implementation, what happens when I give it a vague set of requirements, what happens when I give it a overly detailed set of requirements. I was pretty impressed with what was returned.

CodeWhisperer is something I could see myself getting used to having around - leaving on in the background, forgetting it exists when I’m powering through something and then slowly getting my head around invoking it as I need. There is definitely an art to getting what you want out of CodeWhisperer - I get the feeling that once I have got my head around it though it’d allow me to power through the rudimentary and concentrate more on what matters.

Thank you to the team behind the Builders’ Session content for AIM325 this re:Invent, it was great to see CodeWhisperer in action on my own IDE and get my head around what it’s capable of!


![0.jpeg](images/0.jpeg)