# Overview

I use two laptops. I mostly write codes on my big laptop. This meant that whenever
I went back to my other laptop, there were many changes in my git repositories,
so what I had to do before I wrote this script was to go into every git folder and 
then `git pull` in every single folder. This script automates this.
 
# Example

Suppose you have a folder at your home directory: `~/git` storeing all your
git repositories:

    .
    ├── bash-git-pull-in-every-folder
    ├── bash-visualize-my-math-classes
    └── powershell-graphs-without-internet-access

Open your console and type:
```bash
GitPullInEveryFolder
```
This will automatically `git pull` in every folder on your `~/git` directory.

![GitAllPull](https://user-images.githubusercontent.com/19341857/176710324-6740bd75-4d39-4fa2-b7b5-7f916868322c.png)

# Installation

FYI, it works the same without installation as well.
You can just copy and paste everything on `GitPullInEveryFolder` file
onto your console, and it will work the same.
However, if you want, you could install it:

```bash
# Downloading the script.
sudo dnf install git -y
cd ~/git
git clone https://github.com/soobinrho/bash-git-pull-in-every-folder.git
chmod +x bash-git-pull-in-every-folder/GitPullInEveryFolder

# Running `GitPullInEveryFolder`
cd ~/git
./bash-git-pull-in-every-folder/GitPullInEveryFolder

# (Optional) Adding the script to the `~/.bashrc`
cat >> ~/.bashrc
alias GitAllPull=~/git/bash-git-pull-in-every-folder/GitPullInEveryFolder

# Adding the script to the `~/.bashrc` allows you to
# run `GitPullInEveryFolder` without going to its directory first like this:
GitPullInEveryFolder
```
