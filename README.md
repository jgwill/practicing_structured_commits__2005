# practicing_structured_commits__2005
Practicing what is at : https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines


# --@STCGoal Practice

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
