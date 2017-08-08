# Algebra-1
Tutor worksheets for Algebra 1. Acknowledgements to Robert Culling for the Algebra 1 worksheets from a previous year, which these worksheets are heavily based on.

## Lecture plan
The (core) lecture times are Monday 3pm, Tuesday 10am and Thursday 1pm. The lecture plan (from Wattle, current as of 8 August) is as follows:

Week 1. Laws of Composition, Groups, Subgroups

Week 2. Examples of Groups, Homomorphisms & Isomorphisms

Week 3. Homomorphisms & Isomorphisms, Equivalence Relations, Cosets, Modular Arithmetic

Week 4. The Correspondence Theorem, Product Groups

Week 5. Quotient Groups, generators and relations

Week 6. Abstract symmetry, Operation on cosets, Counting formula

Week 7. Class Equation, actions by quotient groups

Week 8. Rings, Homormorphisms, & Ideals

Week 9. Quotient Rings, Adjoining Elements

Week 10. Product Rings, Fraction Fields, Maximal Ideals

Week 11. Modules, Free Modules, Diagonalising Integer Matrices

Week 12. Generators and Relations, Structure of Abelian Groups

# Using GitHub

A .zip file of the contents can be downloaded by clicking the green button "Clone or download". TeX files can be edited directly by selecting the relevant file, or via software called git.

Hopefully all the .tex files will just compile automagically!

# Using git
A good source on installing and configuring git is https://help.github.com/articles/set-up-git/

You need to use the terminal for the following, use ls and cd to move to the folder you have saved the directory on, see 
https://www.davidbaumgold.com/tutorials/command-line/ moving around the computer section for a tutorial on the command line: 


Copy the online repository to your computer
```
git clone https://github.com/bookbugdonald/Algebra-1
```
This will let you edit the files and make commits 
(i.e. save your work online).

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

Detecting changed files:
```
git status
```
The name of the file you edited will show up RED, this means you have unsaved changes.


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
