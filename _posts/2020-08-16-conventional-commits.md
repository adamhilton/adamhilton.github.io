---
published: false
---
## Conventional Commits

[Conventional commits](https://www.conventionalcommits.org/) is a specification for commit messages. Writing commit messsages that follow a specficiation like conventional commits allows tooling to be built said specification to do things like:

- Generate changelogs from commit messages
- Enforce consistency of commit message structure

Specifications are contracts for tooling to be written around. As for conventional commits, its aim was to give commit messages explicit structure while still being both human readable and easy to understand.

---


### Commit Structure

Here's the basic structure of a conventional commit:
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```


Here are some examples of commits that follow the conventional commit specification.

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