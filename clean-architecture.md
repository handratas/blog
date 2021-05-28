# [Clean Architecture](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship-ebook-dp-B001GSTOAM/dp/B001GSTOAM) by Uncle Bob: Summary
Index:
- [1. What is Design & Architecture](#chapter1)
- [2. A Tale of Two Values](#chapter2)

# <a name="chapter1"></a>1. What is Design & Architecture
- There is no difference between them. None at all. 
- The word “architecture” is often used in the context of something at a high level that is divorced from the lower-level details.
- “Design” more often seems to imply structures and decisions at a lower level. But this usage is nonsensical when you look at what a real architect does(Those low- level details and high-level decisions are part of the whole design of the house).
- So is with software design, you can't have one without the other. There is simply a continuum of decisions from  the highest to lowest levels.

## The Goal 
- The goal of software architecture is to minimize human resources required to build and maintain the required system. 
- If that effort is low, and **STAYS LOW** throughout the lifetime of the system, the design is good. If that **EFFORT GROWS** with each new release, the design is bad. It’s as simple as that.

## Bullet Points
- The only way to go fast, is to go well. 
- Like the story of the Tortoise and the Hare :
- - "Slow and steady wins the race."
- - "The race is not to the swift, nor the battle to the strong."
- - "The more haste, the less speed."
- Modern developers are in a similar race, and exhibit a similar overconfidence. And most of time, their overconfidence will drive the redesign into the same mess as the original project.
- Good, clean, well-designed code matters.
- Familiar lie: "We can clean it up later; we just have to get to market first!"
- The fact is that making messes is always slower than staying clean, no matter which time scale you are using.

## Conclusion
- In every case, the best option is for the development organization to recognize and avoid its own overconfidence and to start taking the quality of its software architecture seriously.

# <a name="chapter2"></a>2. A Tale of Two Values
