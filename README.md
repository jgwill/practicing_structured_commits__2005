# practicing_structured_commits__2005
Practicing what is at : https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines


# --@STCGoal Practice

## Synopsis of Structured Commit

```html
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

## Example

```txt
docs(changelog): update changelog to beta.5
```
```txt
fix(release): need to depend on latest rxjs and zone.js
```

----

# Practicing example and results

## Commit message

```sh
git commit . -m "feat(changelog): atempt to use auto-changelog packag
I tried to generate but the packaging do not seem to be the one

closes #4"
```

## Results and Autogenerated Changelog

* The command executed was : **npm run chglog:generate**

### And the results is the following Markdown in the CHANGELOG: 

```md
## 1.0.1 (2020-05-20)

### Features

* **changelog:** atempt to use auto-changelog package ([d4755d7](https://github.com/jgwill/practicing_structured_commits__2005/commit/d4755d7da01394d09505ed187a9dcb8e878a27e8)), closes [#4](https://github.com/jgwill/practicing_structured_commits__2005/issues/4)
```

## 1.0.1 (2020-05-20)


### Features

* **changelog:** atempt to use auto-changelog package ([d4755d7](https://github.com/jgwill/practicing_structured_commits__2005/commit/d4755d7da01394d09505ed187a9dcb8e878a27e8)), closes [#4](https://github.com/jgwill/practicing_structured_commits__2005/issues/4)

## Observation of the generated feature log

![](https://i.imgur.com/NeO8Mbg.png)

----

----

  This one is type **doc** applied on the scope of **commiting references** and the **subject** was I had added the possible type, scope etc.  
  The Body described a bit what I have done and the **footer** had closed the issue no #1 in the Github issue tab.
```sh
git commit README.md -m "doc(commit ref): added possible type, scope, etc

From the angular commit guideline, I have extracted what I found important.

Closes #1"
```
----

## Possible types

|       |       |       |       |       |
|  ---  |  ---  |  ---  |  ---  |  ---  |
|       |       |   build    |       |  Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)     |
|       |       |       |  Building     |       |
|       |       |   ci    |       |  Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)     |
|       |       |       |  Continuously Integrating changes     |       |
|       |       |   docs    |       |    Documentation only changes   |
|       |       |       |  Documenting     |       |
|       |       |   feat    |       |   A new feature    |
|       |       |       |   Featuring    |       |
|       |       |   fix    |       |   A bug fix    |
|       |       |       |  Fixing     |       |
|       |       |   perf    |       |  A code change that improves performance     |
|       |       |       |   Performing enhancement    |       |
|       |       | refactor      |       |   A code change that neither fixes a bug nor adds a feature    |
|       |       |       |  Better coding     |       |
|       |       |  style     |       |    Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)   |
|       |       |       |   minor    |       |
|       |       |  test     |       |   Adding missing tests or correcting existing tests    |
|       |       |       |  Testing     |       |


# ...

|       |       |       |       |       |
|  ---  |  ---  |  ---  |  ---  |  ---  |
|       |       |   build    |       |  Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)     |
|       |       |   ci    |       |  Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)     |
|       |       |   docs    |       |    Documentation only changes   |
|       |       |   feat    |       |   A new feature    |
|       |       |   fix    |       |   A bug fix    |
|       |       |   perf    |       |  A code change that improves performance     |
|       |       | refactor      |       |   A code change that neither fixes a bug nor adds a feature    |
|       |       |  style     |       |    Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)   |
|       |       |  test     |       |   Adding missing tests or correcting existing tests    |


## Possible Scope

|       |       |       |       |       |
|  ---  |  ---  |  ---  |  ---  |  ---  |
|       |       |   animations    |       |       |
|       |       |   common    |       |       |
|       |       |   compiler    |       |       |
|       |       |   compiler-cli    |       |       |
|       |       |   core    |       |       |
|       |       |   elements    |       |       |
|       |       |   forms    |       |       |
|       |       |   http    |       |       |
|       |       |   language-service    |       |       |
|       |       |   platform-browser    |       |       |
|       |       |   platform-browser-dynamic    |       |       |
|       |       |   platform-server    |       |       |
|       |       |   platform-webworker    |       |       |
|       |       |   platform-webworker-dynamic    |       |       |
|       |       |   router    |       |       |
|       |       |   service-worker    |       |       |
|       |       |   upgrade    |       |       |



## Subject

The subject contains a succinct description of the change:

* use the imperative, present tense: "change" not "changed" nor "changes"
* don't capitalize the first letter
* no dot (.) at the end


## Body (Contrast the Changes)

Just as in the subject, use the imperative, present tense: "change" not "changed" nor "changes". The body should include the motivation for the change and **contrast** this with previous behavior.


## Footer (external system related)

The footer should contain any information about Breaking Changes and is also the place to reference GitHub issues that this commit Closes.

Breaking Changes should start with the word BREAKING CHANGE: with a space or two newlines. The rest of the commit message is then used for this.


----

# Resources

## Related

### Branching to structure a sequence of action

* [Structured Committing Experimentation ref2006021209](http://simp.ly/p/Wfv22J)


## References

### 1. Angular

* Angular/angular. (n.d.). GitHub. Retrieved May 20, 2020, from https://github.com/angular/angular

### 2. Git Commit Message Conventions
* Git Commit Message Conventions. (n.d.). Google Docs. Retrieved May 20, 2020, from https://docs.google.com/document/u/4/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit?usp=embed_facebook

### 3. Conventional-changelog

Conventional-changelog/conventional-changelog. (2020). [JavaScript]. conventional-changelog. https://github.com/conventional-changelog/conventional-changelog (Original work published 2014)
