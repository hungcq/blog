---
title: 'Software Engineering: Technical or Organizational?'
categories:
- essays
- english
date: "2023-07-15T15:05:00+07:00"
tags:
- software-engineering
---

Recently I interviewed with a "top" Internet company in Vietnam. Top, in terms of salary offered, at least.
But the interview content and process, in my opinion, are by no way at the top.
I wonder how their recruitment and HR departments,
which are willing to spend a good deal of money for headhunting services and salary offering,
put so little thought into preparing the interview content and process.
I can summarize the interview of such single-minded organizations in a single word: technical.

So what does it mean when an interview is "technical"?
Of course, technical content, in the normal sense of the word, is necessary.
It ensures a basic level of competency required to do the job, which entails solving technical problems.
For a backend engineer, you probably need to know scaling techniques, main types of databases,
inter-service communication mechanisms, basic DS & algo, etc. But besides these basic technical knowledge,
other things are technical details. They include things like obscure language features,
implementation details of frameworks, random meanings/decisions bound to a particular technology.
They might be useful in some rare cases, such as low-level optimization, writing infrastructure libraries,
or troubleshooting some rare concurrency bugs. However, most of the time, they are mere details.
Details are what you can pick up along the way when it is necessary, provided you know the basics.
You can even take notes of those for easy retrieval when there is a need. But most of the time,
you need to get it out of your head, for they serve no practical purpose,
and they also prevent you from seeing the bigger picture. Let's take some examples.
Should I remember things like different types of GCs, different levels of DB isolations,
or whether Python implementation of map uses chaining or open addressing to handle collisions?
What good does it serve remembering those during my daily work? Is it often the case that you run out of memory,
unless there is a stupid bug in your code? Should you fix the bug or change your runtime GC?
How many times during a given year will you have to create a new DB?
Is DB concurrency bug more prevalent than code bug or operational mistake?
Some companies even ask about the meaning of HTTP error codes again and again.
I assume they are all hardcoders and "browser debuggers",
because they probably don't know that most languages/frameworks offer constants for that,
and API testing with Postman also has the meaning shown for you.

So what, aside from basic technical knowledge, is more important than technical details in software engineering?
The word "engineering" speaks for itself. It is a collaborative activity spanning years or even decades.
Processes, at the organizational level, affect how thousands of people in hundreds of different teams work,
communicate and collaborate. You don't write a piece of code to run once and optimize for 10MB of memories
or 10ms of run time. You write code to be read hundreds of times by others.
You design systems and tests that need to anticipate years of accumulation of changing business requirements.
In such a changing and unexpected environment, everything is a tradeoff.
Obviously, we have trade-offs in business decisions,architectural decisions,
and organizational aspects themselves. But there is also a tradeoff between organizational aspects and technical aspects.
You can spend your time optimizing for 10ms of run time or writing 10 clear, resilient unit tests.
Your leader can spend his time trying to reduce 2 instances of compute resources
or thinking about how to improve automation and quality assurance processes that can reduce the amount of manual work two-fold.
I have been in an engineering organization where thousands of engineers,
all of which can efficiently solve algorithm questions and all can answer with details about different levels of DB isolations,
have little to do each month other than changing about 10 lines of code.
The immediate reason is that we focus on manual testing and complex release processes
instead of improving automation and enforcing quality at the early point of the development cycle.
But the bigger reason behind is that we have been drowned in a sea of details,
unable to put up a good policy and process at the organizational level before it was too late.

So what, after all, is the point of all this analysis (or complaint)?
I'm not hoping that those organizations who label their work "software engineering"
but have little idea of what the word means, to change in the near future.
We can only use this as a guide to distinguish the actual engineering organization from the spurious one,
ideally during the interview process, so we could save our invaluable time and become a better engineer ourselves.