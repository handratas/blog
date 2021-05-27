# Test

## Test Type
- Unit Test: Unit tests are focused and fast.
- Integration Test: verify interaction between parts of your program.
- End-to-end tests: tests verify features, have the highest fidelity, are often instrumented, and may take longer to run.
Unit tests are focused and fast. Integration tests verify interaction between parts of your program. End-to-end tests verify features, have the highest fidelity, are often instrumented, and may take longer to run.

## Test-Driven Development (TDD) 
TDD is a technique for building software that guides software development by writing tests.

In essence you follow three simple steps repeatedly:

1. Write a test for the next bit of functionality you want to add.
2. Write the functional code until the test passes.
3. Refactor both new and old code **UNTIL** it become well structured.

## Test Double
Test double is a general term used by `Gerard Meszaros: xUnit Test Patterns: Refactoring Test Code` to describe any kind of pretend object used in place of a real object for testing purposes.
Using his vocabulary, there are at least five types of Test Doubles:
- [Test Stub](#test-stub)
- [Mock Object](#mock-object)
- [Test Spy](#test-spy)
- [Fake Object](#fake-object)
- [Dummy Object](#dummy-object)

### Test Stub
A test double that verify [indirect inputs](https://handratas.github.io/blog/indirect-input) of SUT with the condition `inputs` is given by tester.

### Mock Object 
A test double that verify [indirect outputs](https://handratas.github.io/blog/indirect-output) of SUT with the condition `inputs(optional) & outputs` is given by tester.

### Test Spy
A test double that verify [indirect outputs](https://handratas.github.io/blog/indirect-output) of SUT with the condition `inputs(optional)` is given by tester.

### Fake Object
A test double that help run (unrunnable) tests (faster).

### Dummy Object
A test double that is only used as attribute or method parameter.
For example: 
- Null 
- "Ignored String"
- new `Object`()
