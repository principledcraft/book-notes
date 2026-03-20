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

The best way to remember things is spaced out repetition. Also helpful is elaboration where you actively think about what you are trying to remember and connecting it to other memories, since memories are stored as part of a network. Strengthening these connections helps retain the memory better.

### Chapter 4 - How to read complex code

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

Research by Janet Siegmund has shown that besides brain areas related to attention and working memory, the brain regions that are activated when writing code are ones related to natural language processing.

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

### Chapter 7 - Misconceptions - Bugs in thinking

Information stored in LTM helps you learn new things, this is called *transfer during learning*. Elaboration, deliberately linking new knowledge to already known concepts helps with transfer during learning. Transfer of learning is when you apply things you have already learned to completely unfamiliar situations.

The amount of learning you can transfer is related to:

* Mastery - How well are the things you already know stored in your LTM
* Similarity - How similar two tasks are.
* Context - How similar the environments are.
* Critical attributes - How clear it is that knowledge is beneficial
* Association - How strong you feel that tasks are similar.
* Emotions - If you feel about something positively, it is easier to transfer that to something new

There are different forms of transfer

* Low road transfer - Unconscious transfer of automated skills
* High road transfer - Conscious transfer of skills
* Near transfer - Transfer of knowledge between domains that are near
* Far transfer - Transfer of knowledge between domains that are further apart, making it less likely that transfer will occur.
* Positive transfer - Occurs when previous knowledge helps learn something new
* Negative transfer - Occurs when previous knowledge hinders learning something new or leads to wrong assumptions.

Transfer is not always given. Research has not shown that skills like chess or programming transfer to higher intelligence or skills in other domains. When learning a new language it might be worth it to pick something radically different as it is more likely to broaden your knowledge.

Paying deliberate attention to similarities and differences when learning a new language can help learn more quickly.

#### Misconceptions

Misconceptions are:

* Faulty
* Held with confidence
* Held consistently across different situations

In order to get rid of a misconception, you don't just need new knowledge, but the faulty knowledge needs to be replaced. This is conceptual change, which is harder than regular learning. Therefore it can be hard to unlearn concepts when learning a new programming language.
Multiple (including incorrect) notions can be present at the same time and pop up again when dealing with more complicated tasks. When being more self conscious (inhibition) a correct notion can prevail over an incorrect one.

Prevent misconceptions when learning new languages by:

* Always keeping an open mind
* Find a list of common misconceptions so you are more aware
* Find people that also learned these programming languages in the same order and ask for advice.

To prevent misconceptions in a new codebase:

* Pair program to test your assumptions
* Run your code and/or use a test suite
* Document common patterns and or misconceptions so others don't fall for the same trap.

## Part 3 - On writing better code

### Chapter 8 - How to get better at naming things

Good names help you better activate things you already know in your LTM. Bad names can cause you to make assumptions, leading to misconceptions.
Naming is also hard, especially when coding and trying to form a mental model, picking an easy name reduces cognitive load.

Phil Karlton, a programmer at Netscape said 'There are only two hard things in programming, cache invalidation and naming things'. Berthold Badler, a professor at Jerusalem University ran an experiment, where the median probability of a variable being named identically was only 7%.

#### Why naming is important

* Names take up a lot of the codebase - 33% of tokens and 72% of characters
* Names appear in code reviews. One in four reviews mention something about a name.
* Names are a form of documentation 
* Names can serve as beacons for forming a mental model

#### Naming things

Simon Butler of Open University in the UK defined a set of semantic conventions for naming (which should help reduce cognitive load according to Hermans):

* Use proper capitalization
* Dictionary words only
* Between two and four words
* Identifier names should not be fewer than eight chars with exception of c, d, e,g, i, in, InOut, j, k, m, n, o, out, t, x, y, z.
* Identifiers should not begin or end in underscores (writers note: I see an exception for Python private vars convention here.)
* No hungarian notation
* Long identifier names should be avoided where possible
* Identifiers should not combine upper and lower case chars in unusual ways
* Identifiers should not be composed of solely a numeric value (e.g. fifty)

It might seem over the top but unnecessary information can cause higher cognitive load. Many programming languages contain naming standards, it's good to adopt those where possible. Allemanis argues that names across codebases should be consistent help with chunking.

Lawrie found that naming does not improve when a codebase evolves, underlining the importance of good naming conventions from the start. Same goes for tests, new developers often copy existing conventions.

Seeing that researchers differ on the right approach we can see how subjective this still is.

Good names help retrieve relevant concepts from your LTM.

Good names can contain:

* Domain knowledge
* Knowledge about programming concepts
* Knowledge about conventions (like using i or j for a counter)

#### When to evaluate your naming

During coding cognitive load is often high, so it is not the best time to evaluate naming. Instead, while reviewing your code you can ask:

* Without knowing the code, are names clear? Do you understand the words used?
* Are any of the names ambiguous or unclear?
* What names are similar, and are their usages also similar or not?

#### What types of names are easier to understand

It has been shown in research (Lawrie, Hofmeister) that identifier names consisting of words are easier to understand and aid in finding bugs faster. However, longer variable names are harder to remember, specifically the number of syllables. It is recommended not to use names with a prefix or suffix.

Apart from a few specific cases, like e.g. s for strings and i,j,n or x,y,z for ints. It has been shown (Beniamini) that there is a wide variability in prescribed meaning of single letter names. Thus it is better to use whole words to improve comprehension.

Camel case has been shown (Binkley) to lead accuracy, with the sacrifice of speed. However, if one is used to camel case they will be slower at snake case and vice versa. If you get to pick a convention, it might be best to pick camel case.

#### Names and bugs

Butler found correlation between pieces of code with bad names and a higher number of bugs. Of course this does not mean causation. It could be written by a novice programmer, or cognitive load when writing this piece of code was high. Bad naming could be a good indicator for code that can be improved. Improving naming can make it easier to solve bugs.

#### Choosing better names

Name molds (Feitelson) - the different ways variables can be represented even though the meaning is the same (e.g. y_max, vs max_y or max_benefit_amount vs benefit_max). Different styles can be used throughout the codebase, discussing it and choosing similar molds can help with comprehension.

Feitelson defines a 3 step model for choosing a name (not necessarily in this particular order):

* Select the concepts to include in the name
  * What does the object used for and what information does it hold and what does it represent (e.g. a unit like m or kg). If there is a comment close to the name, words from the comment should probably be included in the name. Or if input is not validated (unsafe) vs when it is (safe).
* Choose the words that represent these concepts
  * This can vary widely between programmers. A project lexicon in which synonyms are registered for common concepts can help.
* Construct a name using these words
  * Choose consistent name molds across the project. Also format them in a way they occur in natural language. E.g. for 'The maximum number of points' choose 'maximum_points' over 'points_max' or include prepositions like indexOf or elementAt.

### Chapter 9 - Avoiding bad code and cognitive load

Code with code smells is more likely to contain bugs, and it is also more likely to change than code without smells (Foutse Khomh).

Different code smells can cause different effects, some examples:

* Long parameter list, complex switch statements - overload working memory
* God class, long method - Hinder efficient chunking, leads to reading code line by line.
* Duplicate code - Chunking gone wrong. - Similar looking code can be different in practice, leading to misconceptions.

Structural antipatterns - code is correct but not structured on a way to make it easy to work with
Conceptual antipatterns - The code is structured neatly but the names used in the code are confusing.

Arnaoudova describes the following linguistic antipatterns:

* Methods do more than they say they do
* Methods say more than they actually do
* Methods that say the opposite of what they do
* Identifiers that say the contain more than they actually contain
* Identifiers whose names say that they contain less than they do
* Identifiers that contain the opposite of what the entity contains

When studying these in open source codebases it was quite prevalent. E.g. 64 percent of variables starting with 'is' are not boolean. Science confirms that these antipatterns create a higher cognitive load (Fakhoury). It might lead you to retrieve wrong information from your LTM, or make assumptions causing you not to investigate further.

### Chapter 10 - Getting better at solving complex problems

The elements of problem solving:

* The goal state, when the problem is considered solved.
* The start stage, the initial state before problem is solved
* The rules that lay out how we can reach the goal from the start.

Rules of the problem often come in the form of constraints, such as programming language or dealing with already existing functionality.

All steps we can consider while solving a program is called the state space. The problem solver has to select the best path through this space to reach the goal.

Research has consistently shown that generic problem solving methods do not apply and that problem solving is neither a generic skill or a cognitive process because the ability to solve a problem relies heavily on prior knowledge regardless of skill or cognitive ability.

Also when using a generic approach your brain tries to retrieve useful memories, but since the approach is too generic, strategies related to specific ways of solving the problem might not be found. The more specific the connections the better. As covered earlier, knowledge transfer from a domain like chess to mathematics is less likely, as is transfer from a generic domain to a specific one.

#### LTM and problem solving

When solving a problem, your LTM is searched for memories relevant to the problem to be solved.

There are different types of memories

* Procedural or implicit - Unconscious e.g. knowing how to tie shoe laces
* Declarative or explicit - Facts / things you can remember, there are two types:
  * Episodic - How did you experience a situation in the past
  * Semantic - Memory for meaning, concepts or facts.

Implicit memories also play a role when programming, e.g. remembering certain shortcuts or having certain intuition on how to solve a problem.
However, such things can also be hard to unlearn, and thus hinder you when learning something new.

#### Automatization and creating implicit memories

When you do something over and over, you can eventually do it without thinking about it, it takes hardly any extra cognitive energy. This frees up more cognitive capacity to solve bigger and more complex problems. You train these types of memories by repetition. The more implicit memories you have, the easier it becomes to program more complex things.

Declarative knowledge can be practiced with flashcards, however implicit memory is created by repeated practice / doing it.

Implicit memories are formed in three phases:

* Cognitive phase -You have to split the problem up into smaller parts and actively think about each part
* Associative phase - You actively repeat the new information until you see patterns of automatic response emerge.
* You can take the action or process the same type of information without thinking. Thus it will not add to the cognitive load a problem poses.

Gordon Logan argues that automatization works by retrieving memories from episodic memory in the LTM. Retrieving such a memory is easier than actively reasoning about it and using up cognitive load. It might be worth to examine your own implicit skills to know where to improve.

To strengthen these explicit memories, you can practice writing the same thing over and over. Also you could try to adapt existing code to use a new concept to become more familiar with it and comparing the different forms actively. Although this type of practice is not commonly done in programming culture, it can really help strengthen your automatization.
Spaced repetition is key to learning.

#### Learning from code and its explanation

Deliberate practice can improve small programming skills, however it is not enough to become better at problem solving. What you can do to strengthen your problem solving skills is to search for worked examples, where others have already described how they solved a similar problem. It has been shown to improve performance across multiple domains and across age groups.

Germane load is the effort it takes to store what you have learned back to the LTM for future retrieval. Thus it is not the most effective just to solve problems on your own even though this seems counterintuitive. Worked examples allow you to offload some cognitive load, giving you a higher chance that relevant concepts are stored back into the LTM.

Worked examples can include:

* Collaborate with a colleague
* Exploring GitHub and reading code
* Read blogs and books about source code

## Part 4 - On collaborating on code

### Chapter 11 - The act of writing code

Petre and Blackwell defined the cognitive dimensions of notation (CDN) framework, which discusses several activities during programming and their cognitive impact:

* Searching - You are reading an executing code to search for something in particular. This is hard on STM, you have to remember the problem and what avenues of code you already explored.
  * It is best to offload pieces of your cognitive load to notes or a separate document.
  * It can also be helpful to leave little breadcrumbs in the form of comments while searching, especially if you cannot finish the search in one go.

* Comprehension - Similar to search, but here you do not have a good understanding of what the code does in detail.
  * Refactoring can help as well as offloading working memory by e.g. drawing a model, and update it if you learn more.
  * This helps not having to get it from your memory later. It can also help prevent misconceptions.
  * If you continue at a later time, this model can help you get back into the task.

* Transcription - The part where you have a plan and are just coding. Its mainly hard on LTM since you have to recall syntax and patterns for implementation.

* Incrementation - A mix of all three where you search and try to understand the code to later add e.g. a new feature. This is the most common form you encounter as a programmer.
  * Since it encompasses all three, it needs the most support memory wise, especially if you are new to the codebase.
  * Split up a big task in smaller tasks and be deliberate on which subtask you are working on. This can help retrieve relevant concepts from memory.
  * First search, then try to comprehend and only then increment.

* Exploration - Similar to incrementation, when trying out a new concept or blocking out a piece of code.
  * Since it also involves all aforementioned processes, here too offloading can be a good idea, for example by drawing a rough sketch of the concept or a diagram.

Debugging can be described as a mix of all 5 of these activities.

#### Interruptions

Solingen found that 20% of a developers time is spent on interruptions and they can take 15-20 minutes each.
These results were confirmed by Parnin. Also when developers are surveyed 62% indicate that this is a serious problem.

Nakagawa found that the brain indeed seems to warm up and cool down in between tasks, and that the cognitive load in the middle of the task was highest. Therefore it can help to split a problem into smaller subtasks.
Parnin unsurprisingly found that interruptions are quite disruptive to workflow and require re-warming up and re-forming the mental model before coding again.

To better deal with these interruptions it can help to store your mental model in notes, drawings and diagrams. Writing comments has gotten a bad rap, but code itself does not often explain the goal, the why and what alternatives were considered. John Ousterhout puts it as "The overall idea behind comments is to capture information that was in the mind of the designer but couldn't be represented in the code.".

Fred Brooks says on comments that they are most useful for comprehension because they always exist with the code, while retrieving relevant documents takes time and can cause extra cognitive load. Therefore it can be helpful to temporarily store your mental model in a comment when you are interrupted.

Prospective memory is remembering having to do something in the future. Thus it is closely related to problem solving and planning. You can help yourself by leaving TODO comments, sticky notes or email, or having a separate list.

If you divide your task in subgoals and document them, it is easier to return to the task later. Subgoals can also be documented in code and serve as documentation for future implementation by others.

Bailey discovered unsurprisingly that tasks that are interrupted take longer to complete. Also people that are interrupted displayed more anxiety. Thus it is good to actively think about when it is best to interrupt or how to signal if you are busy or not.

#### Multitasking and automatizing

It has been shown over and over again that we cannot effectively multitask. This is if you have not yet reached the implicit memory stage and a second task does not happen almost automatically. Even though, counterintuitively people that multitask often feel very productive. Thus programming while on Slack might not be the best idea.

### Chapter 12 - Designing and improving larger systems

Green, Blackwell and Petre defined a framework to look at the cognitive dimensions of codebases called the *cognitive dimensions of code bases* (CDCB) framework, defining the following dimensions:

* Error proneness - How error prone is the codebase, due to lack of documentation, vague names, or inconsistent conventions. Hanenberg shows that statically typed systems outperformed dynamic ones in terms of time and accuracy of programmers finding bugs.
  
* Consistency - A language, framework or codebase that is more inconsistent in its use of concepts or names can lead to greater cognitive load because it takes longer to understand and find relevant information.

* Diffuseness - How many lines of code or chunks the code needs to express a concept, less diffuse code will lead to better understandability and readability.

* Hidden dependencies - When it is hard to see which parts of the code depend on others e.g., and having to navigate multiple files to trace it or use IDE features to find definitions and usages. This can be partly compensated for with better documentation, but it is always good to have a policy on how to adopt or integrate a new dependency.

* Provisionality - How easy it is to think while using a tool. If a codebase, workflow or language is very strict it can be hard to express new ideas quickly without e.g. dealing with types always. Then the code is not a model of thought, but just of execution. This is especially the case in learning, as you want to be able to think about what you are writing and not all things around it.

* Viscosity - How hard it is to make changes in a certain system. Code that is dynamically typed is easier to change than the statically typed ones. Also code that is not very modular and where a change requires modification in different places can also lower viscosity. In addition, if it takes a long time to compile or test that also has negative effects.

* Progressive evaluation - How easy it is to run or check partial incomplete work. Some systems support live programming (hot reloading) where code can be changed without having to be rerun or recompiled. Another way to do this is to give a library or function some parameters that can be changed while the program is running, thus being able to evaluate changes separately in a live system.

* Role expressiveness - How easy it is to see the role of different parts in a program, e.g. by function name, syntax conventions (e.g. for booleans set vs is_set variable name), or syntax highlighting. Another example is the earlier mentioned linguistic antipatterns. They can also lower role expressiveness and lower understanding.

* Closeness of mapping - How well a programming language or code maps to the domain and problem being solved. Some languages like COBOL or doing things in Excel map closely to the financial domain. For codebases this can be achieved by using names and mapping the software using names and concepts close to the business domain.

* Hard mental operations - Some systems require the user to think very hard. This could be due to use of more difficult programming languages, using a large number of parameters and having to remember the order. Vague names also require harder mental work, or combining two already difficult concepts into a new one. This doesn't have to be all bad and can be a conscious choice, but it is good to beware of the tradeoffs when making decisions.

* Secondary notation - The ability to add comments or keyword names to function calls, providing extra context to the reader and thus making it easier to understand.

* Abstraction - How easy it is for people to create their own level of abstraction in a language. Mostly available in all programming languages now (writers note: maybe this can also be interpreted as how well the system is abstracted, high level concepts that are separated from lower level ones?)

* Visibility - How easy it is to see different parts of the system. E.g. it can be hard to see what parts a system consists of if it is spread over many different locations or files. Return types can also impact visibility e.g. the difference between a string, json and an object in terms of readability and understandability.

#### Design maneuvers and their trade-offs

* Error proneness vs viscosity - If you want users of your code to make fewer mistakes, it is likely that you require them to enter more information. Typing is an example of this. The use of typing will likely reduce errors, but it will make it more work to change the system, thus lowering viscosity.
* Provisionality and progressive evaluation vs. error proneness. The easier it is to work with and run imperfect code, the more likely it is that this code is never properly finished but used instead, increasing the chance of errors.
* Role expression vs diffuseness - Adding additional syntactic elements such as keyword arguments and types can increase role expression, but increase diffuseness.

#### Dimensions and activities

* Searching -  Hidden dependencies can harm searching. Diffuseness causes code to be longer which harms searching. Secondary notation can help searchability.
* Comprehension - low visibility can harm comprehension because it is harder to see how things relate, making understanding harder. Role expressiveness can help comprehension.
* Transcription - Consistency means you will have to fit your code into an existing model, requiring more mental effort.
* Incrementation - Adding new features to a codebase is related to closeness of mapping. It allows thinking about the goal and less about programming concepts.
* Exploration - Explored by good progressive evaluation and provisionality. Hard mental operations and abstractions can harm exploration because they place a higher cognitive load on the programmer (writers note: but doesn't abstraction make it easier? I'd say the lack of abstraction harms exploration).

Knowing which activities will most likely be conducted in the codebase can help you choose the right design decisions. Based on the lifetime of the code the emphasis might also change.

### Chapter 13 - How to onboard new developers

Many software engineers are not trained in onboarding, making the process frustrating for both sides. What typically happens:

* The senior overloads the newcomer with a lot of information
* Then they give the newcomer a task, which the senior views as extremely simple
* which they cannot do due to cognitive load being too high due to missing context, domain knowledge or automatized programming skills or lack of relevant chunks being absent.

As we know, if cognitive load is too high, the capacity to store relevant memories is reduced, making it hard to remember what was taught.

This can be caused by something called the curse of expertise. This is where an expert has forgotten that the knowledge they have which is second nature to them is actually very hard to acquire. This means that they will more often see tasks as easy or trivial.

#### Differences between experts and novices

Experts do not necessarily have all the answers, but they do possess more episodic memories and automatized skills, as well as the ability to perform better chunking, while a novice might have to read the code line by line to form understanding.

#### Neo-Piagetian model for programmers

The model by Piaget for child development can be mapped to programming in the following way:

* Sensorimotor stage - Programmer has understanding of how the program executes, but cannot correctly trace a program.
  * This happens with people with no prior experience, or when switching between radically different languages.
  * It has no use explaining high-level concepts if execution cannot be understood at a low level.

* Preoperational stage - A programmer can predict the outcome of a few lines of code, and often makes guesses of what the code does.
  * They do not oversee larger concepts in the code.

* Concrete operation stage - Programmer reasons about code deductively by reading rather than using induction.
  * Can reason about code based on names, variables, and chunks.
  * Still lacks a complete understanding of entire codebase which makes them unsure about which strategy is the right one, leading them to get stuck on an approach rather than to reflect if that is the right one.
  * Diagrams etc can help here.

* Formal operational stage - Programmer can reason logically, consistently and systematically.
  * Includes reflecting on your own actions, which is essential for debugging.
  * Not so interesting for the onboarding process (writers note: I disagree here, especially if they are new it is helpful for understanding and chunking that the code is structured regardless of experience)

These stages seem to follow one another, but in reality they are mixed. Depending on context, someone might fall back to a lower level for certain tasks compared to others.

#### Seeing concepts concretely vs abstractly

Explanations can be given in very abstract and very concrete terms. Maton showed that beginners benefit from both types of explanations. First the beginner needs to learn the high level concept, followed by a concrete example. Then there should be time to step up again in abstraction level, allowing someone to take the more general abstraction and storing it in their LTM, now having gained a better understanding.

This can go wrong if:

1. Only abstract concepts are used for explanation
2. Only concrete concepts are used for explanation
3. First an abstract explanation is used followed by a concrete one, but then there is no time to go back up one abstraction level, thus not allowing the *repacking* of this information for storage in LTM.

#### Activities to support the onboarding process

It is best to have them do only one task at a time to reduce cognitive load, also due to context switching. A suggestion of a task for each type of activity is given below:

* Exploration - Browsing the codebase to get an overview
* Searching - Finding a class that implements a particular feature
* Transcription - Giving them a very clear plan and having them implement e.g. a new method
* Comprehension - Focused on understanding, e.g. having them summarize a part of the code in natural language.
* Incrementation - Adding a feature to a class, including the creation of the plan for the feature.

The activities listed below can build on each other, and you can switch them up between coding tasks and e.g. learning more about the domain based on prior knowledge and experience.

#### Support the memory of the person onboarding

Patience and empathy is key. Make sure to present all relevant information and concepts both in code and domain and explain them thoroughly, both abstractly and concretely. Having these things will likely also help existing developers by offloading some thinking. Separate learning about the domain from learning about the code. You could even prepare flashcards for both.

What often happens is that existing developers show the code to a newcomer and immediately ask them to implement something. This is likely to fail since the STM is overloaded with both trying to understand the code, the domain and the goal.

Giving them small focussed tasks helps with allowing room to store things in LTM. Also having some summary documentation helps other newcomers and existing developers. They could still implement something, but then eliminate things like searching for the right place. You could prepare that beforehand.

It can be tempting to start by showing diagrams, but as shown before, this is not always helpful. Always evaluate when using this technique and step away from it if the person is not yet at the point when diagrams / drawings etc. are useful.

#### Reading code together

The text comprehension techniques mentioned earlier can also be used when onboarding someone, since applying these techniques (for them) can also reduce their cognitive load.

* Activating - Explain relevant concepts before the code reading session starts
* Determining importance - It can be hard for a newcomer to determine what's important. So pointing out the most important parts beforehand can help.
* Inferring - It can be hard to know details not explicitly mentioned but that have to be inferred. You can point them out or maybe they have already been documented somewhere else.
* Monitoring - Regularly check the level of understanding by asking questions or asking them to give a quick summary of concepts or parts of the code and help them improve their understanding while doing so.
* Visualize - Either ask the newcomer to draw a diagram to further their understanding or prepare it yourself beforehand to help with teaching.
* Questioning - Ask them questions, or encourage them to ask questions as well. When you see they start guessing answers, it is probably a signal that they are starting to suffer from cognitive overload.
* Summarize - A summary of a piece of code can be submitted to the codebase as documentation. This is a good task for a newcomer to do because it also teaches them the general workflow of the codebase.
