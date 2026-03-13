# The Programmers Brain

Felienne Hermans  ·  Manning  ·  August 2021

## Summary

A book that explores the cognitive processes at work while coding that gives practical tips on how to better navigate and reason about code and how to help others reason about your code more effectively.

## Part 1 - On reading code better

### Chapter 1 - Decoding your confusion while coding

Three types of confusion while programming are defined:

* Lack of knowledge
  * The lack of knowledge around concepts or paradigms of programming that block you from starting to comprehend what is happening.
* Lack of easy to access information
  * What is presented in terms of information and how it helps you understand, e.g. a function name that does not give enough information on its own without having to read its content.
* Lack of processing power in the brain
  * Related to the number of variables, operations and steps a piece of code uses to perform a task that make it impossible to keep everything into your working memory at once.

#### Cognitive processes used while coding

Three different processes work together while coding

* Long term memory
  * Holds knowledge that needs to be accessed after a long period of time.

* Short term memory
  * Can temporarily hold concepts while working, like a variable or method name.

* Working memory
  * Where active processing takes place, e.g. making a decision on how to structure a piece of code.

### Chapter 2 - Speed reading for code

Research shows that 60% of a programmers time is spent on understanding code, not writing it. Short term memory only has a size of two to six elements, thus you have to rely on knowledge in your LTM.

When you have more knowledge about the programming language and/or certain patterns, you have to rely less on reading low level code but can instead read it in chunks, making you read faster. Experts can remember more bits of code than beginners, supporting that theory. When processing random information, they are equally fast.

Code can contain elements that make it easier to progress, such as design patterns, comments and beacons, e.g. variables and function names.

### Chapter 3 - How to learn programming syntax quickly

It is important to know quite a bit of syntax, because having to look it up will slow you down.

A good way of practicing this syntax is the use of flash cards.
You can expand the set of flash cards as you encounter new things, and thin them out once you feel you have mastered some of them.

It's good for your memory to actively try to retrieve a bit of information from memory before trying to look it up. 

The best way to remember things is spaced out repetition. Also helpful is elaboration where you actively think about what you are trying to remember and connecting it to other memories, since memories are stored as part of a network. Strengthening these connections helps retrain the memory better.

### Chapter 4. How to read complex code

Short term memory is used to remember things, while your working memory is used to process information. Both STM and working memory can hold 2 to 6 items at a time. When a problems contains too many elements that cannot be divided into chunks, the working memory gets overloaded.

Three types of cognitive load are distinguished:

* Intrinsic load: how complex is the problem itself
* Extraneous load: what outside distractions add to the problem
* Germane load: load by having to store memories in LTM (discussed later)

If your working memory is overloaded, it's worth to check which type of cognitive load you are experiencing so you can address it.

It might be nice to create different functions for behavior and put them in different files. But this delocalisation of behavior can also add extra cognitive load.

There are several ways to reduce load:

* (Cognitive) refactoring - Refactoring can make code easier to understand, but it's not always more maintainable in the long run. So you could refactor temporarily, just to get a better mental picture. An example of this is inlining code of a function call. This type of refactoring is often meant for a single person. If they turn out valuable, they can always be merged.
* Replacing unfamiliar language constructs - If you have a hard time understanding part of the syntax you could temporarily replace that syntax with a more familiar one to help understanding. These are also nice to add to the flashcards mentioned previously.
* Creating a dependency graph or creating a state table can help you more effectively reason about a piece of code. Tracking and highlighting a variable or function call throughout a longer version can also help you piece together how it is used.
