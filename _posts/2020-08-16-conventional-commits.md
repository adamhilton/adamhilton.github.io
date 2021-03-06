---
published: false
---

## What are conventional commits?

[Conventional commits](https://www.conventionalcommits.org/) is a specification for commit messages. Writing commit messsages that follow a specficiation like conventional commits allows tooling to be built said specification to do things like:

- Generate changelogs from commit messages
- Enforce consistency of commit message structure

Specifications are contracts for tooling to be written around. As for conventional commits, its aim was to give commit messages explicit structure while still being both human readable and easy to understand.

---


## What do conventional commits look like?

Here's the basic structure of a conventional commit:
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```


So what Here are some examples of commits that follow the conventional commit specification.

```
feat(api): allow coffee to be drank

This should allow users to want to drink coffee the ability to do so.

resolves #123
```

```
refactor: move coffee manager into mug namespace
```

```
fix(database): allow multiple affects of coffee to be inserted into user record

User could only have one affected stat inserted at a time due to not accounting for multiple effects of coffee object.
```

```
feature: add ability to drink large or small espresso

Users can now specify if they want to drink a large or small espresso by invoking one of two new drink espresso methods.

BREAKING: `User#drinkEspresso()` has been removed. Use either `User#drinkSmallEspresso()` or `User#drinkLargeEspresso()` instead

resolves #124
```