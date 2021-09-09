# Code Smells
Index:
- [1. Introduction](#part1)
- - [Chapter 1 - What is Code smells](#chapter1)
- - [Chapter 2 - How can you create code smells?](#chapter2)
- [2. Types of Code Smells](#part2)
- - [Chapter 3 - Bloaters](#chapter3)
- - [Chapter 4 - Structured Programming](#chapter4)

# <a name="part1"></a>1. Introduction
## <a name="chapter1"></a>What is Code smells
- Code smells is a characteristic in code that possibly relate to a deeper problem, such as when you need to change something in ONE place in your code, but you need to make a changes in many other places.
- Code smells are key signs that refactoring is necessary. In the process of refactoring, we get rid of smells, enabling further development of the application with equal or greater speed.

## <a name="chapter2"></a>How can you create code smells?
- The lack of regular refactoring, can lead to a complete paralysis of a project over time, wasting a few years of development and requiring you to spend several more years to rewrite it from scratch.
- Therefore, it is necessary to get rid of code smells while they are still small.

# <a name="part2"></a>2. Types of Code Smells
## <a name="chapter3"></a>Bloaters
- Bloaters are code, methods and classes that grows and become enormous overtime as your program evolves (especially when nobody makes an effort to keep it clean).
- They make code bigger than it need to be in the places you use them.


### <a name="chapter3.1"></a>Long Method

