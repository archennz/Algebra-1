# Algebra-1
Tutor worksheets for Algebra 1

# Using git

Copy the online repository to your computer
```
git clone https://github.com/bookbugdonald/Algebra-1
```
This will let you edit the files and make commits 
(i.e. save your work online).

Edit something then type
```
git status
```
The name of the file you edited will show up RED, this means you have unsaved changes.

When you are working on an EXISTING repository you can save a lot of pain by always refreshing your local copy using
```
git pull
```
You will get all of the latest changes and this will usually prevent clashes from occuring.

Saving your work has two stages: COMMIT them to your local repository and then you PUSH to the online repository.
These are the commands you need:

## Making a commit

Do this to save your latest changes to your computer:
```
git commit -a -m"a messsage about the commit"
```
This will add all of your changes to a commit and save the message in git describing your changes.
The message is useful if you want to find some work that was deleted!

If you have added a NEW file then you will need to tell git about it using
```
git add [NAME OF FILE]
```
Do this BEFORE you do `git commit`.

## Pushing changes

Do this to update the online copy of the repository- so everyone can see your changes.
```
git push
```

## Dealing with merges

Sometimes git will tell you that you can't push to the online repository because your local copy is out of date.
In that case you have to do `git pull` BEFORE you can do `git push`.

Usually git is clever enough to synchronise your work without requiring extra input.

If it is not then it will list conflicts: files with conflicts will have sections inserted between rows of `>>>>>>>>`.
You need to choose which of the sections is correct and then do a new commit.
The commit message might look a bit weird but that's ok!
