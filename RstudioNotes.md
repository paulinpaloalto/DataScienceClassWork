# Notes about Using RStudio
As a new user of *RStudio*, it's useful to keep a log of interesting tips and techniques as they appear.
## Working with Files, Directories and Projects
*RStudio* has the concept of a *Projec*t, which is very useful for managing multiple activities that you want
to work on in parallel. The simplest way to view this is as an elaboration on the notion of folder or
directory: you can define a project from an existing folder someplace on your local machine.
* Select "New Project" on the "File" pulldown menu
* Choose an existing folder and name it as a *Project*
* *RStudio* will track various state for you automatically, including your current R working data 
(saved in the file *.RData* in the
root folder of the *Project*).
* When you switch between projects, *RStudio* will ask whether you want to save the current working data.
Then it will autoload the saved *.RData* file from the project to which you just switched.
* As you write R code, e.g. functions, one easy way to manage this process is to store each function as a separate source
file in the local project directory, e.g. *foo.R*. Then you can edit these either with an editor within *RStudio* or your editor of
choice on the local file system.
* When you want to test the function, just say
<br>
 > source('foo.R')
<br>
 > val = foo(param1, param2)
 

