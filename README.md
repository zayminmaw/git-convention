# Git Convention

Multiple people will be working on this project so we will need to have a common ground on git. A common language that makes it easier to debug issues across project boundaries. This will be a great help for generating CHANGELOGs, too.

You can read [here](https://www.conventionalcommits.org/en/v1.0.0-beta.2/#specification) by yourself.

Here is the summary. Read the above link for more details.

**Important**: for every feature release and fix (except hotfix) always make your own branch first and pull request. After you task is done always checkout back to main branch, pull the update and make a new branch to work on your next task.

### Branch Name Format

**minor**/description (for new feature) <br/>
**patch**/description (for fix) <br/>
**major**/description (for breaking change fix or feature) <br/>
**feature**/description (for breaking change feature) <br/>

### Commit Format

In commit messages format we will be using 

```
<type>(optional scope): <description>

[optional body]

[optional footer]
```

**`<type>`** as in 

`build` Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)<br/>
`ci` Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)<br/>
`docs` Documentation only changes<br/>
`feat` A new feature<br/>
`fix` A bug fix<br/>
`hotfix` A direct fix to main branch<br/>
`perf` A code change that improves performance<br/>
`refactor` A code change that neither fixes a bug nor adds a feature<br/>
`style` Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)<br/>
`test` Adding missing tests or correcting existing tests<br/>
`BREAKING CHANGE` As the name suggest for breaking change<br/>

**`[optional scope]`** as in where is the changes being made and this is optional. <br/>

**`<description>`** as in summary of your change. <br/>

**`[optional body]`** as in more detailed explanation. <br/>

**`[optional footer]`** as in additional references. <br/>


### Syntax

To submit multiline commits you can use 

```
git commit -m "message-1" -m "message-2"
```

### Suggestion

`git add .` is fine and all and easy but it won't help us track or trace the commits. We strongly encourage you to use `git add 
<file-name>` and commit each file instead.

