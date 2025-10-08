# dev-notes
Here I out thoughts about setup, practices I like, and things worth remembering.

## Things I like

* **Create things that matter.** Optimize for the timeframe that actually matters. If we’re shipping a long-lived, large-scale app, follow solid engineering practices. If a tiny, temporary feature is needed by three people, an Excel might be enough.
* **Building is a last resort** Often there is another way to achieve the same outcome. Then don't do it.

## Dev setup

* WSL (Ubuntu) + VS Code WSL extension.
  Fast installs/builds, Windows conveniences (GCM, Visual Studio), repos checked out in WSL. Great for running different agents.

## Filestructure
* Feature slicing
* Files < 100 lines of code
* Methods < 15 lines of code 

## Backend
* .NET for heavt stuff 
* Node/typescript for smaller

## Infra

* Terraform
* RBAC (no long-lived keys)

## Testing

* Pragmatic. Tests should deliver net business value. Often as fast as manual regression if done right.

## Front-end

* [Bulletproof React](https://github.com/alan2207/bulletproof-react) — practical feature-sliced structure. Usually enough.

## AI

* Use where it clearly contributes. Requirements-driven dev can work well with good architecture.
* Amazon Q CLI is great for cost; call Codex/Claude Code as sub-agents when needed.
* Automatic PR reviews with strong models are great.
* Daily log-monitoring agents belong in every team.

## Git aliases

These save a surprising amount of effort. Put in `~/.bash_aliases` on Linux.

```bash
alias gsw='git switch'
alias gswc='git switch -c'
alias gpl='git pull'
alias gps='git push'
alias gci='git commit -am'
alias gadd="git add ."
alias gbr='git branch'
alias gst='git status'
```
