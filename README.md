# dev-notes
Here i document my thoughts on setup, practices I like and other things worth reminding myself about

## Things I like
### Creating things that matter.
 - I want to do things that is effective on the timeframe that matter the most.

When building a large scale enterprise app that should be used by thousands of users +10 years, then all of the best software engineering practices should be followed. But within that maybe we have a small non-critical feature that will be used by 3 people temporarily, then I will send them an excel if it solves the issue.

- Not building something. If someone asks me something, and there is a way to save many hours by not doing it whilst still getting the intended effects then I will argue my point.

### Dev setup
 - WSL with Ubuntu and VS Code WSL extension
This works unexpectedly well even for modern dotnet development. Being able to run Windows with all of the conveniences that comes with that (git-credentials-manager, Visual Studio etc) but having the machine run really quickly with builds and installs. It's great. Repos checked out in WSL. Especially important with all of the differnet agents.

### Backend
Feature slicing
Dotnet

### Infra
Terraform
RBAC - no keys

### Testings
Pragmatic testing, focus on what is important. Tests should be a net positive in terms of buisiness value. Often writing tests can be as fast as manual regression testing. 

### Front-end
[Bulletproff React](https://github.com/alan2207/bulletproof-react) also works for other frameworks. Practical example of feature slicing. Don't need much more.

### AI
Use where it contributes. Requirements driven development is great for some things.  Combine with good architecture and it can work. 
Amazon Q CLI is great per cost. Can call Codex/Claude Code as subagents for when other models are needed. 

Automatic PR reviews with the strongest models is amazing.
Agents that do monitoring of logs daily should be in every dev team.


## Git aliases
These I use, saves unexpectedly much effort. Put in .bash_aliases if using Linux
```
alias gsw='git switch'
alias gswc='git switch -c'
alias gpl='git pull'
alias gps='git push'
alias gci='git commit -am'
alias gadd='git add .'
alias gbr='git branch'
alias gst='git status'
```
