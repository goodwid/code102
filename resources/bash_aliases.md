(See the keyboard shortcuts in [the repo Readme](../README.md) for help creating these new hidden files.)

Copy the following small block to your `.bashrc` file (this file may not exist; you may have to create it):

``` bash
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi
```

Create a new file in your home directory called `.bash_aliases`, then copy the large text block below into the file and save it.

``` bash
#
# directory aliases
#

alias ll='ls -l'
alias lla='ls -la'
alias cd..='cd ..'


#
# git aliases
#

alias ga='git add'
alias gc='git commit -m'
alias gpo='git push origin'
alias gs='git status'


#
# class-centric aliases
#
# change this to the full directory where your Code 201 classwork exists

alias 201='cd ~/Documents/Code201/labwork'

#
# bash management aliases
#

alias edbash='vi ~/.bashrc'
alias edal='vi ~/.bash_aliases'
alias newdot='source ~/.bashrc'
```

Finally, type `source ~/.bashrc` to reload the file. (You'll need to retype this any time you change the `.bashrc` or `.bash_aliases` files in order to get the changes to be available.)
