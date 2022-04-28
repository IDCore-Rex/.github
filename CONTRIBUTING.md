# Contributing Guidelines

First off, thank you so much for taking the time to contribute. All contributions are more than welcome!

## Boyscout Principle

We follow the Boyscout Principle or Boyscout Rule to help ensure the maintainability of our code bases.
The original Boyscout Rule reads as, "Always leave the campsite cleaner than you found it.". You may have
heard this adapted for software as principle expressed as, "Always leave the code better than you found it."
The purpose of this principle is to help reduce tech-debt through small consistent efforts in every pull request.

In general

- If you're working in an area of code that is not tested please provide tests.
- If you need to refactor code try to make things consistent.
- Follow the principles laid out in the [12 Factor App](https://12factor.net/)
- Follow the [SOLID Design Principles](https://dev.to/ezzy1337/a-pythonic-guide-to-solid-design-principles-4c8i) when refactoring.
- Commented code should be deleted with extreme prejudice.
- If there is a more efficient way to implement a function make it more efficient.


## Structured commit messages

- Limit the subject line to 72 characters
- Capitalize the first letter of the subject line
- Use the present tense ("Add feature" instead of "Added feature")
- Separate the subject from the body with a blank line
- Reference issues and pull requests in the commit body


## Coding style guide

We are using ESLint to ensure a consistent code style in the project, based on [Airbnb's JS style guide](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base).

Some other ESLint plugins are also being used, such as the [Prettier](https://github.com/prettier/eslint-plugin-prettier) and [Jest](https://github.com/jest-community/eslint-plugin-jest) plugins.

Please make sure that the code you are pushing conforms to the style guides mentioned above.


## Tests

We encourage a test driven approach to software development. That being said we understand not every developer wants to follow strict TDD disciplines.
To bridge the gap we ask that every PR be accompanied with tests that prove the bugfix/feature functions work as expected.

**You need to include tests**

- If you are adding net new code.
- If you are implementing a bugfix with existing tests. (At the very least the existing tests should be updated for the bugfix)
- If an modifying a section of code that was previously untested please provide tests for that code.

**You DON'T need to include tests**

- When you are making developer changes (i.e. refactoing that doesn't introduce new functionality, doc changes etc.)


## Pull Request Process

- When creating a pull request please fill out the template provided as best as you can.
At a minimum, complete the definition of done checklist and provide a brief description
of what the PR accomplishes (i.e. what bug it resolves or feature it implements).
- Pull Requests require approval by at least 1 of the code owners before they can be merged.
- Pull Requests should be merged into the `main` branch.
