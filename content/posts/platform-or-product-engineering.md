---
title: 'Platform or product engineering?'
categories:
- essays
- english
date: "2025-03-03T21:35:00+07:00"
tags:
- software-engineering
---

Recently, I interviewed with a self-advertised "top" company,
with the initial assumption that they were a decent engineering organization.
However, the actual technical interview they conducted proved me totally wrong.

The interview lasted around 55 minutes,
with around 25 minutes of product discussion and Q&A with a manager whose English was incomprehensible.
But let's just consider that part unfortunate and unimportant,
and focus instead on the actual 30-minute technical discussion,
which I think was insightful in terms of software engineering and product development in general.

If I had only 30 minutes to know how much a person knew about modern software engineering,
what would I discuss? Probably incremental development, continuous delivery and learning,
domain modeling and refactoring, quality control, technical and organizational scalability,
site reliability, and some other things I can't think of now (my bad).

These matters can be explored through direct high-level questions
or discussed in the context of a concrete example.
I initially thought the latter was the case when I was asked to design a Document Search service.
But what the interviewer tried to get at was anything but a service useful in some way to the product and end users:
how I would design a scalable vector search database,
and how I would implement batch processing and a map-reduce engine.
What followed was a series of miscommunications between two people thinking at different levels of abstraction - 
me thinking about choosing the appropriate tools for the job,
and him trying to build "scalable," general-purpose platforms.

Which brings me to my main point:
what should be the focus of an engineer building software products for a particular domain?
It should never be platform building, which is one level of abstraction below the requirement.
The hallmark of progress in all domains of thought is an increasing level of abstraction.
We think less about unimportant details, abstract them away, take them for granted,
then use them as tools to solve higher-order problems.
Where would geometry be if every proof required a demonstration of the Pythagorean theorem?
Where would software engineering be if we were still working with assembly language?
Granted, assumptions and theories are challengeable, abstractions sometimes leak,
and platforms sometimes don't meet all our needs and require adjustments.
But only minor changes and tricks are justifiable, not major modifications and rebuilds, because:
1, The cost of building and testing a new platform is too high, especially for a product team, and
2, If the original tool is so bad for our purpose, why did we choose it in the first place?

The product engineers who take on such platform-building endeavors are, at best, wasted assets.
The companies that value such technical "skills" will probably end up with average products
built by a bunch of average engineers - never skilled enough,
but always thinking they are working for a PaaS company.