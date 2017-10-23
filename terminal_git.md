## How to use git?

This is a short intro in the most basic features for using GIT. It's not complete and you will come accross problems you cannot solve. So use those further references and tutorials to get to know more about GIT 😉

Feel free to use those references:
[Git Cheat Sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
[Getting Started](https://git-scm.com/book/en/v1/Getting-Started)

## Why GIT?

GIT is a version-controll-system. It's great because...

(1) if you break your program, you can always role back to a version that worked.
(2) you can work together with multiple programmers who are working on the same project at the same time.

How does it work? It's basically a folder. We can initialize GIT in every folder we would like to. After initializing, GIT will keep track of all changes we do (e.g. adding some code or deleting it).

Let's get started. 😶

## Initialize and Clone

*Heads up: You have to have GIT installed in your system.*

There are two ways you can get started. Choose the right one for you:

(1) You want to start yourself: Move to the folder with your project and type `git init`. This will activate GIT in your folder.
(2) You clone a repository from a friend: Move to the folder you want to download the project in and type `git clone <LinkToRepo>`.  You will get the LinkToRepo from your friend.

## The very basic workflow

I recommend to use those commands in this order:

(1) `git pull`: Start with `git pull` every time you start working on your project. This will make sure, you always have the latest changes.
(2) `git status`: After a change, figure out, what has changed using `git status`. It will show you all files that have changed.
(3) `git add <filename or foldername>`: You have to select the files that you want to commit in the next step. All the one's that you have not selected, will not be commited.
(3) `git commit -m "Write some Message"`: This will commit your change. Imagine it like saving the next version of your app. This will set a reference to the current state that will be written to the "log". So you will always be able to come back to this state.
(4) `git push`: This will share your current state with the main repository (e.g. Github). So other people can access it.

If somebody else has pushed in the meantime, you have to pull again. 😛

## Merge conflicts

**What is a merge conflict?**
When trying to push, you might have to pull. What happens now is: Two people have changed the same project. Most the time, GIT will merge the two changes together. But imagine both have changed the same file 😱. Now we have to decide who's changes should win the conflict.

GIT cannot decide for us. It will now show an error and will tell us, which file the conflict happened.

Open this file. You will see something like:

```
<<<<<<<<<<<<<<<<<<<<<<<<< HEAD
YOUR CHANGE
======================
CHANGE FROM YOUR FRIEND
>>>>>>>>>>>>>>>>>>>>>>>>>
```

**How to handle merge conflicts?**
Delete one of the changes or keep both. But make sure to delete those strange looking lines:
```
<<<<<<<<<<<<<<<<<<<<<<<<< HEAD
```
```
======================
```
```
>>>>>>>>>>>>>>>>>>>>>>>>>
```

After deleting the lines and deciding which code you want to keep, you have to commit again.

You would do `git add <FilesThatHaveChanged>` and `git commit -m "Merge."` and now you do `git push` 🎊 and it worked. (hopefully)
