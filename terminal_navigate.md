## How to navigate in the terminal

The terminal is a program that helps you to access files and other programs. You can think of it as "Explorer for Developers".

The very basic: You can run a program by writing it's name. There is a program for everything.

Let's try. There is a program for showing your username. Type `whoami` in the terminal.

*Good to know*: In documentations there is often a `$` to make clear, that this line of code should be written in the terminal. Example: `$ cd newProject` and you should write in your terminal `cd newProject`.

## Programs to navigate

The most important programs to navigate are:

- `cd` - short for "Change Directory" you use it to switch to another folder. Usage: `cd path_to_folder`
- `ls` (Mac/Linux) /`dir` (Windows) - short for "List" / "Directory" will list all folders and files in the current directory.
- `pwd` - short for "print working directory" will show you the path to the folder you are currently in.

Let's try. Type `pwd` afterwards type `ls`.

## Pathnames

If you just type `cd` there will not happen a lot. You would like to describe a path where you want to go.

What is a path?
In Linux and Mac, pathnames will start with a single `/`. So the folder for the downloads would be in `/Users/myname/Downloads`.
In Windows it's slightly different. Pathnames will start with `C\:` (or another letter). So the folder for wonloads would be in `C:\Users\myname\Downloads`.

*What is a bit tricky*: Linux/Mac uses a simple slash `/` between foldernames. Windows uses a backslash `\`. Keep this in mind when copying code from the internet. :wink:

So let's have a try. There are some important ways to describe a path that you should know about:

- `foldername/subfolder/` - this is the very basic way to describe a path. You would use it like `cd foldername/subfolder`. This would change your current directory into the subfolder.
- `..` - this will bring you up the parentfolder. Let's say you are currently in `foldername/subfolder`. `cd ..` would bring you into the folder `foldername`
- `.` - this is the current folder.
