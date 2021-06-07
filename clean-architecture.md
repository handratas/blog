# [Clean Architecture](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship-ebook-dp-B001GSTOAM/dp/B001GSTOAM) by Uncle Bob: Summary
Index:
- [1. Introduction](#part1)
- - [Chapter 1 - What is Design & Architecture](#chapter1)
- - [Chapter 2 - A Tale of Two Values](#chapter2)
- [2. Starting with the Bricks: Programming Paradigms](#part2)
- - [Chapter 3 - Paradigm Overview](#chapter3)
- - [Chapter 4 - Structured Programming](#chapter4)

# <a name="part1"></a>1. Introduction
## <a name="chapter1"></a>Chapter 1 - What is Design & Architecture
- There is no difference between them. None at all. 
- The word “architecture” is often used in the context of something at a high level that is divorced from the lower-level details.
- “Design” more often seems to imply structures and decisions at a lower level. But this usage is nonsensical when you look at what a real architect does(Those low- level details and high-level decisions are part of the whole design of the house).
- So is with software design, you can't have one without the other. There is simply a continuum of decisions from  the highest to lowest levels.

### The Goal 
- The goal of software architecture is to minimize human resources required to build and maintain the required system. 
- If that effort is low, and **STAYS LOW** throughout the lifetime of the system, the design is good. If that **EFFORT GROWS** with each new release, the design is bad. It’s as simple as that.

### Bullet Points
- The only way to go fast, is to go well. 
- Like the story of the Tortoise and the Hare :
- - "Slow and steady wins the race."
- - "The race is not to the swift, nor the battle to the strong."
- - "The more haste, the less speed."
- Modern developers are in a similar race, and exhibit a similar overconfidence. And most of time, their overconfidence will drive the redesign into the same mess as the original project.
- Good, clean, well-designed code matters.
- Familiar lie: "We can clean it up later; we just have to get to market first!"
- The fact is that making messes is always slower than staying clean, no matter which time scale you are using.

### Conclusion
- In every case, the best option is for the development organization to recognize and avoid its own overconfidence and to start taking the quality of its software architecture seriously.

## <a name="chapter2"></a>Chapter 2 - A Tale of Two Values
- Every software system provides two different values to the stakeholders: **behavior(function)** and **structure(architecture)**.
- Software developers are responsible for ensuring that **both** values remain high. Often times we focus on one to the exclusion of the other or even more the lesser of the two values.

### Behavior
- Programmers are hired to make machines behave in a way that makes or saves money for the stakeholders. 
- We do this by helping the stakeholders develop a functional specification, or requirements document. 
- Then we write the code that causes the stakeholder’s machines to satisfy those requirements. When the machine violates those requirements, we debug and fix the problem.

### Architecture
- Software was invented to be “soft.” It must be **easy** to change the behavior of machines. When the stakeholders change their minds about a feature, that change should be simple and easy to make.
- If we think `new requirement` from stakeholders as a shape, architectures should be as shape agnostic are practical.
- The difficulty in making such a change should be proportional only to the scope of the change, and not to the shape of the change.
- Bad architecture signs: software developers often feel putting new requirement to existing feature as if they are forced to jam square pegs into round holes.

### The Greater Value? Behavior or Architecture?
- If you ask **business managers**, they’ll often say that it’s more important for the software system to work **(behavior)**.
- If you ask **developers**, they often go along with business managers even if they should be saying **architecture**, because:
- - If you give me a program that works perfectly but is impossible to change, then it won’t work when the requirements change, and I won’t be able to make it work. Therefore the program will become useless.
- - If you give me a program that does not work but is easy to change, then I can make it work,
and keep it working as requirements change. Therefore the program will remain continually useful.
- Even if there's no such thing as a program that is impossible to change, they could be *practically* impossible due to cost of change exceeds the benefits of change.

### Eisenhower's Matrix
`I have two kinds of problems, the urgent and the important. The urgent are not important, and the important are never urgent.`

![Eisenhower's Matrix](https://user-images.githubusercontent.com/12756891/120153338-ce3c6400-c218-11eb-99bf-8acba8b7c36b.png "Eisenhower's Matrix")

There is a great deal of truth to this old adage. Those things that are urgent are rarely of great importance, and those things that are important are seldom of great urgency.
- The first value of software—behavior—is urgent but not always particularly important.
- The second value of software—architecture—is important but never particularly urgent.

We can arrange these four couplets into priorities:
1. Urgent and important
2. Not urgent and important (Architecture)
3. Urgent and not important (Behavior)
4. Not urgent and not important

Note that Architecture is in 2nd position, and Behavior is 3rd position. \
**And the mistake** is that business managers and developers often make is to elevate items in position 3 to position 1. \
It is the responsibility of the software development team to assert the importance of architecture over the urgency of features.

### Fight For The Architecture
- Fulfilling this responsibility means wading into a fight—or perhaps a better word is "struggle". The development team has to struggle for what they believe to be best for the company(architecture), and so do the management team, and the marketing team, and the sales team, and the operations team. *It’s always a struggle.*
- Remember, as a software developer, you are a stakeholder. You have a stake in the software that you need to safeguard. That’s part of your role, and part of your duty. **And it’s a big part of why you were hired.**
- This challenge is doubly important if you are a software architect. Software architects are, by virtue of their job description, more focused on the structure of the system than on its features and functions. Architects create an architecture that allows those features and functions to be easily developed, easily modified, and easily extended.
- Just remember: If architecture comes last, then the system will become ever more costly to develop, and eventually change will become practically impossible for part or all of the system. If that is allowed to happen, it means the software development team did not fight hard enough for what they knew was necessary.

# <a name="part2"></a>2. Starting with the Bricks: Programming Paradigms
Paradigms are ways of programming, relatively unrelated to languages. A paradigm tells you which programming structures to use, and when to use them.

To date, there have been three such paradigms: 
- Structured Programming
- Object-Oriented Programming
- Functional Programming

## <a name="chapter3"></a>Chapter 3 - Paradigm Overview
### Structured Programming
- The first paradigm to be adopted (not the first to be invented), discovered by `Edsger Wybe Dijkstra` in 1968.
- It emerged in the late 1950s with the appearance of the ALGOL 58 and ALGOL 60 programming languages.(not discovered yet) [source](https://en.wikipedia.org/wiki/Structured_programming)
- **Structured programming imposes dicipline on direct transfer of control.**

### Object-Oriented Programming
- Discovered in 1966 (2 years before Structured Programming discovered) by Ole Johan Dahl and Kristen Nygaard.
- These two programmers noticed that the function call stack frame in the ALGOL language could be moved to a heap, thereby allowing local variables declared by a function to exist long after the function returned. The function became a constructor for a class, the local variables became instance variables, and the nested functions became methods. This led inevitably to the discovery of polymorphism through the disciplined use of function pointers.
- **Object-oriented programming imposes discipline on indirect transfer of control.**

### Functional Programming
- First to be invented in 1936 by Alonzo Church who invented l-calculus. L-calculus is the foundation of LISP language in 1958 by John McCarthy. A foundation notion of l-calculus is **immutability**-that is, notion that the values of symbols do not change. This also effectively means a functional languange has no assignment statement(most of functional language do have some means to alter value of a variable, but only under very strict dicipline).
- **Functional programming imposes discipline upon assignment.**

### Food For Thought
- Notice each of the paradigm *removes* capabilities from the programmer and none of them adds new capabilities. 
- Each imposes some kind of extra *dicipline* that is negative in its intent. The paradigm tell us what *not to do*, more than they tell us what *to do*.
- The three paradigm together remove ***goto* statements**, **function pointers**, and **assignment**.
- Is there anything left to take? In the many decades that have followed, no new paradigm have been added. It can means these 3 paradigms are likely to be the only three we will see.

### Conclusion
- We use polymorphism as the mechanism to cross architectural boundaries. 
- We use functional programming to impose discipline on the location of and access to data.
- We use structured programming as the algorithmic foundation of our modules.
- Notice how well those three align with the three big concerns of architecture: **function, separation of components, and data management.**

## <a name="chapter4"></a>Chapter 4 - Structured Programming

