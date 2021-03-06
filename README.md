# Overview

I use two laptops. I mostly write codes on my big laptop. This meant that whenever
I went back to my other laptop, there were many changes in my git repositories,
so what I had to do before I wrote this script was to go into every git folder and 
then `git pull` in every single folder. This script automates this.
 
# Example

Suppose you have a folder at your home directory: `~/git` storeing all your
git repositories:

```bash
home
└── soobinrho
    └── git
        └── college-programming
        └── dotfiles-personal
        └── powershell-graphs-without-internet-access        
```

Open your console and type:
```bash
PullGitAll
```
This will automatically `git pull` in every folder on your `~/git` directory.

![PullGitAll](https://user-images.githubusercontent.com/19341857/176871556-f7368e41-43b2-4331-954c-5d6054e07c95.png)

# Installation

FYI, it works the same without installation as well.
You can just copy and paste everything on `PullGitAll` file
onto your console, and it will work the same.
However, if you want, you could install it:

```bash
# Downloading the script.
sudo dnf install git -y
cd ~/git
git clone https://github.com/soobinrho/bash-git-pull-in-every-folder.git
chmod +x bash-git-pull-in-every-folder/PullGitAll

# Running `PullGitAll`
cd ~/git
./bash-git-pull-in-every-folder/PullGitAll

# (Optional) Adding the script to the `~/.bashrc`
cat >> ~/.bashrc
alias PullGitAll=~/git/bash-git-pull-in-every-folder/PullGitAll

# Adding the script to the `~/.bashrc` allows you to
# run `PullGitAll` without going to its directory first like this:
PullGitAll
```

<br>
<br>
<br>

