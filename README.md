My Bash Prompt
===========

Open Terminal

Paste in the following:

cd to ~

type `nano .bash_profile`

Paste in the following:

```
#Load in the git branch prompt script.
source ~/.git-prompt.sh

PS1="\[\e[38;5;242m\]\[\e[1m\]\h\[\e[0;37m\]:\[\e[38;5;16m\]\[\e[1m\]\W\[\e[0;37m\]@\[\e[38;5;52m\]\T\[\e[38;5;24m\]\$(__git_ps1)\[\e[38;5;37m\]$\[\e[38;5;235m\] "
```

Looks like: ![]()
