# Dive into the BDD

> TDD (Test-Driven Development) and BDD (Behavior-Driven Development) are both software development methodologies that focus on testing during the development process. While TDD focuses on testing at the unit level, BDD focuses on testing at the behavior level.

> TDD is often used to write unit tests for classes and methods. The process involves writing a test case before writing the actual code, running the test to see it fail, and then writing the code to make the test pass. TDD encourages developers to write code that is testable, modular, and loosely coupled, making it easier to maintain and refactor code over time.

> BDD, on the other hand, focuses on testing the behavior of the system as a whole, rather than individual components. BDD tests are written in a natural language format that is easily understood by both technical and non-technical stakeholders. BDD is often implemented using frameworks such as Cucumber or JBehave, which allow developers to write tests in a Gherkin syntax that describes the behavior of the system in terms of scenarios and steps.

### Gherkin Syntax

``` Gherkin
Feature: Guess the word

  # The first example has two steps
  Scenario: Maker starts a game
    When the Maker starts a game
    Then the Maker waits for a Breaker to join

  # The second example has three steps
  Scenario: Breaker joins a game
    Given the Maker has started a game with the word "silky"
    When the Breaker joins the Maker's game
    Then the Breaker must guess a word with 5 characters

```
