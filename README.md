# Introduction
My rules for commit format

Based on  [Angular`s rules](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#-commit-message-guidelines) and [eegkno/commit_message_format](https://github.com/eegkno/commit_message_format)

Correctly formatted commits are easy to read, which leads to a **readable changelog**. This is why it is important.

> NOTE: every single commit denotes one logical change. [Check this article](https://en.wikipedia.org/wiki/Logical_connective)
# Commit Message Format

### Commit Layout
```
<type>(<scope>): <subject> <fix>: used to reference issue tracker IDs.

<body>: used to explain the what and why of a commit, not the how. Wrap the body at 72 characters in each line.
```

The **scope** (but rly recommended), **body** and **footer** are optional

Some samples: 
```
feature(core): add request API
```

```
docs(changelog): update changelog to beta.5
```
```
fix(release): need to depend on latest rxjs and zone.js (#154)

The version in our package.json gets copied to the one we publish, and users need the latest of these.
```
### Type

- **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
- **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
- **config**: Config only changes
- **docs**: Documentation only changes
- **feature**: A new feature
- **fix**: A bug fix
- **perf**: A code change that improves performance
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **test**: Adding missing tests or correcting existing tests
- **tweaks**: For small changes on other places (please do not use often)
- **misc**: Anything not covered by the above categories, e.g. rename or move files

### Subject 

The subject contains a succinct description of the change:

- use the imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize the first letter
- no dot (.) at the end
- limit to 50 characters

### Scope

The area must contain the modified one (if one), otherwise indicate the logical area that has undergone changes

> In smaller projects, you can use a freer form, but don't overdo it.








