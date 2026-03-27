# Code that fits in your head

Mark Seemann · Pearson · November 2021

## Summary

## Chapter 1 - Art or Science

It is hard to pick a good metaphor when talking about the profession of software engineering / programming. If you compare it with building a house, it will go wrong because:

* Software is not a project with a start and an end, most software keeps evolving and responding to external factors.
* You are continually planning and executing in loops, not in predefined phases.
* You can start pieces that depend on each other out of order if you want. You might miss opportunities if you always build from the bottom up.

Gardening might serve as a better metaphor where:

* Software is a living organism and you need to tend to it, it keeps evolving.
* You need to prevent code rot rather than just taking away dead plants and weeds retroactively

Yet, it is not perfect because

* Software doesn't just grow on its own, it's a deliberate action.

There are other metaphors such as accounting for technical debt and it being akin to other kinds of writing. None of the metaphors are completely wrong, but none are perfect.

### Software as a craft

A good term for it is software craftsmanship, as it encompasses skilled work. How to solve a problem is often situational, and you can learn by doing as well as by gained experience.

It can be beneficial to switch companies often, as you quickly pick up on new skills and techniques and different parts of programming, like frontend, backend, or machine learning. It is similar to the concept of journeyman years where a craftsman would travel around and hone their craft.

The problem with the journeyman model however is that it doesn't scale as it would take a long time before someone becomes a journeyman and mastery is still several years out after that.

Still it is useful to explore guidelines (heuristics) when writing software and teaching others that.

Software should be an engineering discipline but due to the rise of personal computers there were many people that self taught how to program, that they could ignore the body of knowledge already existing.

Software, unlike other forms of engineering, is principally a design activity, as constructing it is basically free compared to construction in the real world.

Real engineering comes from following a set of methodologies that lead to success. We don't have to follow meticulous planning since building software is relatively cheap. However, there is other methodologies we can follow, as outlined in this book.

These are based on experience and what works, rather than a universally scientifically proven set of laws. Software engineering is not like other engineering disciplines, but we can still learn from them.

## Chapter 2 - Checklists

Using a checklist as a memory aid frees you up to focus on the more important parts, offloading the trivial things. It's important that it does not become a measure of performance, or leave an audit trail. It should lead to increased performance without needing increased skill.

### Starting a new codebase

A deliberately rough checklist for new codebases is:

* Use git - it allows experimentation with your code.
* Automate the build (writes note: and deploy) - Easiest to do if there is little code, do this as soon as possible.
* Turn on all error messages - Use linters, code styling tools and other early warning systems and turn them all on, make warnings errors. It is easy to do in the beginning, much harder. It can also serve as a sort of automated quality gate, making it harder to argue against if it was agreed upon at an earlier stage.

## Chapter 3 - Tackling complexity

Software should be engineered in such a way that the process becomes more predictable, and it should sustain the organisation for years or decades. Without an internal eye for quality it soon becomes difficult to deliver in a reasonable timeframe.

Software should provide value. But that does not mean that all code should add value directly, for example, security or internal quality changes also add value in the long term. Therefore we should find a middle ground between just focussing on adding direct value and only focussing purely on the latest technology. This will make software sustainable in the long run.

### Why programming is difficult

Likening a computer to a brain is not a good metaphor. Computers are exact, while thinking, associations and memory can be forgotten or manipulated. While a computer can hold many things, the short term memory can only hold 2-7 concepts at the same time. Throughout the book, the number seven is used as a guideline.

You spend more time reading than writing code. To write new features or fix a bug you must first understand what is already there. Therefore, you must optimize code for readability. Code that is hard to understand slows you down, but code that is easy to understand speeds you up tenfold.

When writing code you are aware of the context in which you write it. Later, when you read it again, all that context is gone, and all that remains is the code. Readable code cannot be written just based on intuition, you need checklists, heuristics etc.

### Intellectual work

Programming involves a lot of unconscious mental activity. You can be "in the zone" and produce code without deliberate awareness. Kahneman's model of System 1 (fast, automatic, error-prone) and System 2 (slow, deliberate, effortful) applies to programming. System 1 is always running in the background trying to make sense of code, but it jumps to conclusions easily (like the bat-and-ball problem where most people answer 10 cents instead of the correct 5 cents).

Because System 1 only works with currently activated information (what you see is all there is — WYSIATI), code should be organised so that all relevant information is visible at the same time. This explains why global variables and hidden side effects make code hard to understand — they are not visible when looking at a piece of code, so System 1 does not account for them.

### Towards software engineering

Software engineering should support the organisation and allow changes at a sustainable pace. Computer science can help but is not the same as software engineering, just as physics is not mechanical engineering. Results from computer science (sorting algorithms, data structures) can be packaged into reusable libraries — you don't need to understand B-trees to query a database.

The remaining challenge is to organise code so that it fits in the human brain. Code must be humane: small, self-contained functions with fewer than seven dependencies, cyclomatic complexity at most seven, and so on. The number seven is used throughout the book as a proxy for the brain's working memory limit.

Software engineering should be the deliberate process of preventing complexity from growing. This may feel like it slows you down, but as Rainsberger puts it, you probably need to slow down — the faster you type, the more code everyone has to maintain. Code is not an asset, it is a liability. Its by applying good architecture that you can maintain a sustainable pace.
