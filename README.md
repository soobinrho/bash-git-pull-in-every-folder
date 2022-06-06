# Overview

I use two laptops. I mostly write codes on my big laptop. This meant that whenever
I went back to my other laptop, there were many changes in my git repositories,
so what I had to do before I wrote this script was to go into every git folder and 
then `git pull` in every single folder. This script automates this.
 
# Example

Suppose you have a folder at your home directory: ` ~/git` storeing all your
git repositories:

    .
    ├── bash-git-pull-in-every-folder
    ├── bash-visualize-my-math-classes
    └── powershell-graphs-without-internet-access

Open your console. Go to the directory you store your repositories: `cd ~/git`
and use the codes at `GitPullInEveryFolder`. This will `git pull` in every folder.

How exactly can you do that? You can just copy and 
paste everything inside `GitPullInEveryFolder`
on your terminal. 

I, however, personally use it 
as the following:

```
# It works the same without installation -- you can just copy and paste everything 
# inside `GitPullInEveryFolder`, but - for your information - you could use it this way.

# The first time you use this:
sudo dnf install git -y
cd ~/git
git clone https://github.com/soobinrho/bash-git-pull-in-every-folder.git
chmod +x bash-git-pull-in-every-folder/GitPullInEveryFolder

# Everytime I use it:
cd ~/git
./bash-git-pull-in-every-folder/GitPullInEveryFolder
...
