# Contributing Guidelines

First off, thank you so much for taking the time to contribute. All contributions are more than welcome!

## Boyscout Principle

We follow the Boyscout Principle or Boyscout Rule to help ensure the maintainability of our code bases.
The original Boyscout Rule reads, "Always leave the campsite cleaner than you found it.". You may have
heard this adapted for software as principle expressed as, "Always leave the code better than you found it."
The purpose of this principle is to help reduce tech-debt through small consistent efforts in every pull request.

In general

- If you're working in an area of code that is not tested please provide tests.
- If you need to refactor code try to make things consistent.
- Follow the principles laid out in the [12 Factor App](https://12factor.net/)
- Follow the [SOLID Design Principles](https://dev.to/ezzy1337/a-pythonic-guide-to-solid-design-principles-4c8i) when refactoring.
- Commented code should be deleted with extreme prejudice.
- If there is a more efficient way to implement a function make it more efficient.


## Commit Best Practices

- Commit early and often.
- Each commit should result in a successful build if cherry-picked into another branch.
- Use the present tense ("Add feature" instead of "Added feature") in commit messages.
- Reference issues and pull requests in the commit body (This is useful for the Github -> Jira integration)
- Before submitting a PR clean-up your commit history. (i.e. run `git rebase -i origin/main`)


## Coding style guide

We are using ESLint to ensure a consistent code style in the project, based on [Airbnb's JS style guide](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base).

Some other ESLint plugins are also being used, such as the [Prettier](https://github.com/prettier/eslint-plugin-prettier) and [Jest](https://github.com/jest-community/eslint-plugin-jest) plugins.

Please make sure that the code you are pushing conforms to the style guides mentioned above.


## Testing

Tests are required for every PR that meets one of the following conditions.

- If you are adding net new code.
- If you are implementing a bugfix with existing tests. (At the very least the existing tests should be updated for the bugfix)
- If an modifying a section of code that was previously untested (This is part of the Boyscout Principle)

Test Driven Development (TDD) is encouraged, however we understand not every developer wants to follow strict TDD disciplines
and there are times when you need to prototype functionality to understand how a feature will work. In such cases strict TDD
is a hinderance. You choose when you write your tests but tests will be required.


## Pull Requests & Code Review Process

- Pull Requests (PRs) should target the `main` branch.
- A Pull Requests (PR) is needed for each feature, bugfix, or developer change.
- A PR should only contain commits specific to a **single** feature, bugfix or developer change. This makes it easier
  to review and to revert the change in the event it breaks something.
- When creating a PR it is **required** the PR Template is filled out completely. If you're confused about any part of
  the template you can read the [PR Template FAQ](https://idcore.atlassian.net/wiki/spaces/IDCORE/pages/9043982/Pull+Request+Template+FAQs)
- PRs require approval from at least 1 code owner before they can be merged.
  - If your PR has gone more than a 24 hours without a review please tag a maintainer to review it.
- All conversations on the PR need to be resolved before it can be merged. This is just a way to ensure the author and
  reviewer have come to an agreement on all the comments, and questions left during code review.
