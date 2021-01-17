# Standards for Effective Developer Collaboration
#### Methods and tools to effectively work together with many developers on one project
## The problem:

We can build software in many different ways - which is definitely a great thing! But with great power comes great responsiility, and although you may not need to adhere to a strict standard of code - you need to at least be in agreement with your team about how to go about developing software and working together.

## This document:

... will talk about some of the workflows and tools a team can use to keep sanity at acceptable levels when collaborating in software development.

# Section 1 - Clean Code

If a software developer could read only one book, the book to read would be [Clean Code by Robert Martin](https://enos.itcollege.ee/~jpoial/oop/naited/Clean%20Code.pdf). It would be beyond the scope of this document to provide a detailed exposition of the work, so we will settle for a modified quick summary from [wojteklu/clean_code.md](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)

> Code is clean if it can be understood easily – by everyone on the team. Clean code can be read and enhanced by a developer other than its original author. With understandability comes readability, changeability, extensibility and maintainability.
_____________________________________

## General rules
1. Follow standard conventions.
2. Keep it simple stupid. Simpler is always better. Reduce complexity as much as possible.
3. Boy scout rule. Leave the campground cleaner than you found it.

## Design rules
1. Keep configurable data at high levels. 
2. Prefer polymorphism to if/else or switch/case. [Reference](https://medium.com/@shanikae/polymorphism-explained-simply-7294c8deeef7)
3. Use dependency injection. [Reference](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)
4. Follow Law of Demeter. A class should know only its direct dependencies. [Reference](https://medium.com/better-programming/demeters-law-don-t-talk-to-strangers-87bb4af11694)

## Understandability tips
1. Be consistent. If you do something a certain way, do all similar things in the same way.
2. Keep your code in line-of-sight. [Reference](https://medium.com/@matryer/line-of-sight-in-code-186dd7cdea88)

## Names rules
1. Choose descriptive and unambiguous names.
2. Make meaningful distinction.
3. Use pronounceable names.
4. Use searchable names.
5. Replace magic numbers with named constants.

## Functions rules
1. Small.
2. Do one thing. [Reference](https://www.freecodecamp.org/news/an-introduction-to-the-basic-principles-of-functional-programming-a2c2a15c84/)
3. Use descriptive names.
4. Prefer fewer arguments.
5. Have no side effects.
6. Don't use flag arguments. Split method into several independent methods that can be called from the client without the flag.

## Comments rules
1. Always try to explain yourself in code.
2. Don't be redundant.
3. Don't add obvious noise.
4. Don't use closing brace comments.
5. Don't comment out code. Just remove.
6. Use as explanation of intent.
7. Use as clarification of code.
8. Use as warning of consequences.

# Section 2 - Version Control

Git is essential for any team working synchronously on a single codebase. It keeps each developer focused on their work without needing to worry about changes being made by their co-developers, while also allowing for easy resolution of conflicts when completed features are ready to be incorporated into the working codebase.

The best book available come from the git website itself written by git evangelists [Scott Chacon](https://www.oreilly.com/pub/au/3843) and [Ben Straub](https://www.oreilly.com/pub/au/6519) - [Pro Git](https://git-scm.com/book/en/v2)

## When to use git

**All projects must use git.** A project may be a monorepo (everything in one repository) or a polyrepo (different features/services spread across different repositories). **No exceptions.**

<!--
TODO:

Link other .md files (relative links) about each technology/standard;

- Git
- Docker
- SQL
- Web Standards
- HTML
- CSS
- JS
- Laravel - API
- Laravel - BO / FO & BO
- Vuejs
- Nuxt.js
- Prestashop
- Wordpress

Learning more frameworks will be essential for creating standards of collaboration in those frameworks.

Roadmap:

- Shopify
- Express
- NoSQL
- Angular
- React

--!>
