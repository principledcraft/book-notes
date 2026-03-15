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

Short term memory is used to remember things, while your working memory is used to process information. Both STM and working memory can hold 2 to 6 items at a time. When a problem contains too many elements that cannot be divided into chunks, the working memory gets overloaded.

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

## Part 2 - On thinking about code

### Chapter 5 - Reaching a deeper understanding about code

#### Variable frameworks and roles

In order to understand code better it helps to use a variable framework like the one defined by Jorma Sajaniemi, that divides variables into 11 categories: Fixed value, stepper, flag, walker, most recent holder, most wanted holder, gatherer, container, follower, organizer and temporary. Classifying each variable in the piece of code can help you understand it better and communicate more effectively about it.

Apps Hungarian notation  (Charles Simonyi) is often wrongly understood to mean you put the type of a variable in front of it, e.g. strName. However, in the original proposal it goes much deeper, like putting c in front for Count, or min/max for minima and maxima. Even though it's not popular today, there is still value in having a shared convention.

#### Gaining a deeper knowledge

Nancy Pennington defined different levels of understanding computer programs. Text knowledge is understanding the syntax of a particular piece of code and being able to read what the program is doing. Plan knowledge is understanding not the individual lines of code, but the intent behind them, which is often concepts not only hidden in keywords and variables, but how parts of the code are related to each other and why.

Jonathan Sillito has defined a typical four step process on how understanding about code is formed:

* Finding a focal point in code
* Expanding knowledge from that focal point
* Understanding a concept from a set of related entities
* Understanding a concept across multiple related entities.

Some techniques and frameworks like dependency injection (and, writers note, also microservices with poor boundaries!) can fragment focal points making it harder to form an understanding. You will have textual knowledge, but it's harder to form plan knowledge. 

This technique can be applied concretely by e.g:

* Circling all variables
* Link similar variables
* Circle all methods and function calls
* Link methods/functions to their definitions
* Circle all instances of classes
* Draw a link between classes and their instances

#### Reading text is similar to reading code

Research by Peter Siebel has indicated that around 60% of a programmers work is spent with reading code, yet not a lot of programmers practice reading it. Because we lack techniques to read code more effectively, we often read it line by line, which leads to *i'll build it myself*, because it's easier to write new code than to understand existing code.

Research by Janet Sigmund has shown that besides brain areas related to attention and working memory, the brain regions that are activated when writing code are ones related to natural language processing.

Chantal Prat showed that, surprisingly, mathematical ability is far less of a predictor for programming ability than your ability to process natural language. Working memory was the best predictor overall.

Similar to reading text, it has been shown by Hidetake Uwano that programmers read 70% of a piece of code in the first 30% of time, which means that they will scan it first instead of reading it line by line.
Experts are more experienced in following the call stack while reading unknown code, while novices read line by line. Apparently tracing the call stack is a skill that has to be acquired with experience.

There are several text comprehension strategies that can be applied to code:

* Activating: Actively thinking about related things to retrieve prior knowledge
* Monitoring - Keeping track of your understanding of a text
* Determining importance - Deciding what parts of a text are most relevant
* Inferring - Filling in facts that are not explicitly given in the text
* Visualizing - Drawing diagrams of the read text to deepen understanding
* Questioning - Asking questions about the text at hand
* Summarizing - Creating a short summary of a text


### Chapter 6 - Getting better at solving programming problems

#### Using models to think about code

Mental models can help communicate to others about the code, as well as offload some cognitive load when your working memory is almost full. They also help retrieve relevant memories from LTM. Using different types of models that focus on different aspect of the problem can help you focus your attention. Not all models are equally helpful, which model you use impacts the time you take to solve a problem and how effectively you do so.

Mental models create an abstraction in working memory which helps you reason about the problem at hand. Models can also work against us, for example when stepping through a highly optimized piece of code, it is likely that it will not execute the way we had originally envisioned.

#### Characteristics of mental models

* Mental models are a simplification of reality. They can be useful if irrelevant details are abstracted away.
* Mental models can change, are not stable. Parts of the model can also be forgotten if people do not engage with it enough.
* Multiple mental models can coexist with each other even if they contradict. Novices can also hold incorrect mental models that are locally coherent but not globally.
* Mental models can be weird and feel like superstitions. People can believe things that do not really make sense.
* People are frugal when using mental models, because they take a lot of energy (e.g. people rather run again to check if it works now than to reason about it).

When learning a new model, it will not always fully replace an old mental model. In situations of high cognitive load, you might thus fall back on an old incorrect model.

#### Mental models in working memory

Johnson-Laird described mental models as being held in working memory. Having an abstract mental model helps you reduce cognitive load when reasoning about code. Having a more concrete mental model with more details makes it easier to reason about the code at hand.

To create a mental model of complex code you can:

* Begin with local models
* List all objects in the codebase and the relationship between objects
* Answer questions about the model and use those to refine the model further

#### Mental models in LTM

Dedre Gentner and Albert Stevens considered models being stored in LTM and they can thus be retrieved when needed, similar to how schemata and connected ideas are stored in LTM. These can also be trained with flash cards: think about e.g. data structures, design and architecture patterns and diagrams. Besides training, it can also be used as an index if you are unsure which pattern to apply.

Mental models both exist in working memory and LTM and those in working memory are influenced by those in LTM.

#### Notional machines

A notional machine (as coined by Ben du Boulay) is the correct and consistent abstraction of the execution of a programming language, even though it might not fully represent reality. They differ from mental models as those can be incorrect and inconsistent. The more you learn about a programming language, the closer your mental model comes to the notional machine. A notional machine is the abstraction we use to reason about a computers functioning at a level that's needed at any given time. Many notional machines can be used at the same time; they can also build on top of each other and be expanded upon. Sometimes, different notional machines can conflict or cause confusion, so it is worth thinking about which notional machine you use. Wrong abstractions can still stay in LTM and thus pop up in working memory.

Notional machines can abstract things at different levels, e.g. programming language vs bytecode. It's important to realise which details you are abstracting away when using notional machine since these might be relevant to the problem you are solving.

Notional machines are often used in communication about code.
When choosing a notional machine to communicate with someone, it's important to try to use terms they might be familiar with, as it relates to the already formed schemata in LTM.

Notional machines are not semantics, as semantics try to formalize programs precisely using mathematics, not abstract notions.
