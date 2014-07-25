My MacOS Bash Prompt
===========

Open Terminal, paste this in and hit enter:

```
cd
touch .git-prompt.sh
nano .git-prompt.sh
```

Now open your browser and navigate to [this link](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh). Copy everything (command + A) on this page to your clipboard.

Go back to Terminal and paste the contents of your clipboard to `.git-prompt.sh` which is the file you left open.

Save and get out of `nano` by hitting `control + x` it will ask you to confirm, type `y` and enter.

Now open your bash_profile by pasting this into your Terminal:

```
nano .bash_profile
```

Once you're in your .bash_profile, paste in the following:

```
#Load in the git branch prompt script.
source ~/.git-prompt.sh

PS1="\[\e[38;5;242m\]\[\e[1m\]\h\[\e[0;37m\]:\[\e[38;5;16m\]\[\e[1m\]\W\[\e[0;37m\]@\[\e[38;5;52m\]\T\[\e[38;5;24m\]\$(__git_ps1)\[\e[38;5;37m\]$\[\e[38;5;235m\] "
```

Save and get out of `nano` by hitting `control + x` it will ask you to confirm, type `y` and enter.

Close Terminal and reopen it.

Now it should look like: 

![Screenshot of my bash prompt](https://raw.githubusercontent.com/atotalpirate/bash_prompt/master/img.png)

Displaying:

* \h = Abbreviated hostname
* \W = Current directory
* \T = Time when that command was entered
* \$(__git_ps1) Current Git branched checked out 
