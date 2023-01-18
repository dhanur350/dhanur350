## Difference between `git reset --hard` and `git revert <shaHere>`
tl;dr: ,There is a very great significance of using `revert` instead of `git reset` coz it preserver all history and its important if you pushed earlier commmit to public and want it to be undone(remove) and still don't want to force push then `git revert` rocks coz it does exactly that! Read below like for more insights!.

## [Source](https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/#undo-a-public-change)  

## - Do u know that if your repo does not accepting changes updates via git pull, you can use git pull -f and it'll forcefully update your current repo with github database of your repo 
## Git push -f will forcely push your repo to Github , but only use this when your git refuse to push it into your repo
## Made a gacp function in bash alias, Windows 

- `gac (){`

    `echo + git add .`
    
    `git add .`
    
    `echo + git commit -m \'$@\'`
    
    `git commit -m "$*" # gac life is amazing adders`

`}`

# Usage: gacp life is super amazing. 
- `gacps shortcuts life to project pushing quicker.`

gacp (){

    echo + git add .
    
    git add .

    echo + git commit -m \'$@\'
    
    git commit -m "$*"

    echo + git push -f
    
    git push -f

}

## Do you know that you can manage two githubs at same computer using this technique

### User1 github handler

Host User1 github.com

    HostName github.com
    
    User git
    
    IdentityFile ~/.ssh/id_rsa_User1 

### User2 github handler

Host User2 github.com

    HostName github.com
    
    User git
    
    IdentityFile ~/.ssh/id_rsa_User2
    
<!--
**dhanur350/dhanur350** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:


- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...

-->
