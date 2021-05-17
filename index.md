# Hi

I'm Handrata, an App Developer since 2013. Currently enjoying creating Android App using Kotlin.

Often times it's hard to separate time between work, family and pursuing knowledge. So, I want to make a note to myself and hopefully useful to others as well.

Add me in [LinkedIn](https://www.linkedin.com/in/handrata-samsul-1517904b/)

Article List:
- [Test](#test)
- [Framework vs Library](https://handratas.github.io/blog/framework-vs-library)

## Test

### Test-Driven Development (TDD) 
TDD is a technique for building software that guides software development by writing tests.

In essence you follow three simple steps repeatedly:

1. Write a test for the next bit of functionality you want to add.
2. Write the functional code until the test passes.
3. Refactor both new and old code **UNTIL** it become well structured.

### Test Double
Test double is a general term used by `Gerard Meszaros: xUnit Test Patterns: Refactoring Test Code` to describe any kind of pretend object used in place of a real object for testing purposes.
Using his vocabulary, there are at least five types of Test Doubles:
- [Test Stub](#test-stub)
- [Mock Object](#mock-object)
- [Test Spy](#test-spy)
- [Fake Object](#fake-object)
- [Dummy Object](#dummy-object)

#### Test Stub
A test double that verify [indirect inputs](https://handratas.github.io/blog/indirect-input) of SUT with the condition `inputs` is given by tester.

#### Mock Object 
A test double that verify [indirect outputs](https://handratas.github.io/blog/indirect-output) of SUT with the condition `inputs(optional) & outputs` is given by tester.

#### Test Spy
A test double that verify [indirect outputs](https://handratas.github.io/blog/indirect-output) of SUT with the condition `inputs(optional)` is given by tester.

#### Fake Object
A test double that help run (unrunnable) tests (faster).

#### Dummy Object
A test double that is only used as attribute or method parameter.
For example: 
- Null 
- "Ignored String"
- new `Object`()
