# Lab 4 report

This lab focuses on making changes to files in a github repository and pushing them to remote source control. Using vim, we try to make the process as fast as possible. All of these screenshots have been taken from the terminal, where the series of commands are run.

1. Logging into ieng6 machine: `ssh asadwelkar@ieng6.ucsd.edu <enter>`
Since I have the ssh key setup on my laptop, I can skip logging in with my password.  
![Image](login.png)  
2. Cloning my fork from my Github account: `git clone git@github.com:ucsd-cse15l-s23/lab7.git <enter>`  
On the ieng6 machine, I have a git access token setup, so I can clone with `ssh`.
![Image](git-clone.png)  
3. Running the tests to see they fail:  
First we navigate into the newly cloned lab7 directory: `cd lab7`  
I make sure I am in the right directory by running `pwd`. Then, we run the bash script to examine the test results: `bash test.sh <enter>`  
The `testMerge2` test fails while the other test passes.  
![Image](failedtests.png)  
4. Editing the code file, this the series of keystrokes: `43 j 11 l x i 2 <esc> : w q <enter>`  
Using the least amount of keystrokes to get to the right line and make the change. `43 j` moves me down to line 43, `11 l` moves me to the correct character in the line, `x i 2` replaces in the `2` in the `index2` with a `1` to make it `index1`. After making the change, I press `<esc>` and then `:wq <enter>` to save the new changes.  
![Image](edit-code.png)  
5. Running the tests to see they now succeed: `bash test.sh <enter>`  
![Image](successtests.png)  
6. Committing changes to fork, series of commands: `git add ListExamples.java <enter>`, then `git commit -m "fixed test" <enter>`, then `git push origin main <enter>`  
We stage the `ListExamples.java` file, commit it with the message "fixed test", and then push to origin.  
![Image](gitaddcommit.png)  
![Image](gitpush.png)  
