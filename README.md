# code-repository-standards

This repo provides best-practice guidelines you'll be expected to follow when developing projects at Stylist. Depending on the application you may notice some rules documented here aren't stricly enforced which is especially true for legacy applications. All new projects or applications should be developed according to the rules documented here.

## Working with GitHub

### Pull Request etiquette 

Assign at least two (or more) developers to your PR, and always endeavour to read anything you're assigned, even if it's not your core focus. In general we write JavaScript, C# and PHP, and it's all code at the end of the day. We've found that the PR is a great place to learn and discuss functionality.

### Each repo should have a pull request template

If the project you're working on doesn't have one, please add one!

### Commit early and often

You're only an SSD failure or a pub thief away from having your work lost, there's no reason not to commit and push things up!

### The Model

At Stylist we favour the git branching model developed by Vincent Driessen – sometimes referred to as git flow (although that name actually refers to a set of CLI tools developed to help with the branching operations for this model).

If this is unfamiliar to you, he has an excellent write up explaining it all in detail. It will be beneficial to [familiarise yourself with this](https://nvie.com/posts/a-successful-git-branching-model/), so that you understand the rationale behind it and what its aims are.

Below is a diagram showing the outline of the model:

![The Model](https://nvie.com/img/git-model@2x.png)

Depending on the application we usually have 3 deployment environments:

**Production** – this is the live site, deployed from a tagged/published master branch – considered 'stable'.

**Preprod** and/or **Staging** – this usually contains master branch, this is where we perform QA, apply fixes and verify that all is ok before deploying to production

**Develop** or **PR** - typically contains work in progress...

## Documentation

Document everything. If possible, write documentation before you even start coding. Where appropriate, make sure your project's documentation covers :

* functional specification (as a user I can...)
* technical specification (flow diagrams, infrastructure requirements)
* detailed instruction of how to use and set up locally (repo's README.md)

When developing APIs use tools like [API Blueprint](https://apiblueprint.org/) or [Swagger](https://swagger.io/). 

When developing code, document interfaces/contracts, classes and methods using syntax specific to the programming language choosen:

* [C#](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/xmldoc/recommended-tags)
* [PHP](https://developer.wordpress.org/coding-standards/inline-documentation-standards/php/)
* [JavaScript](https://developer.wordpress.org/coding-standards/inline-documentation-standards/javascript/)

## Testing

Test Driven Development approach is recommended but it's not mandatory. You will however be expected to write a testable code according to SOLID and DRY principles. There's a lot of tutorials and resources available online about how to write a testable code. One example can be found [here](https://dashdevs.com/blog/writing-testable-code-main-rules/).

At Stylist you'll be responsible for writing unit and integration tests for your new and existing applicaitons as well as e2e tests where appropriate.

## Coding

At Stylist we don't currently enforce strict coding style guides, however you'll be expected to write clean code according to best practice rules specific to the programming language choosen: 

* [C#](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)
* [PHP](https://github.com/inpsyde/php-coding-standards)
* [JavaScript](https://github.com/airbnb/javascript)