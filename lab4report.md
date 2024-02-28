# Lab 4 report

This lab focuses on making changes to files in a github repository and pushing them to remote source control. Using vim, we try to make the process as fast as possible. 

1. Logging into ieng6 machine: `ssh asadwelkar@ieng6.ucsd.edu <enter>`  
![Image](login.png)  
2. Cloning my fork from my Github account: `git clone git@github.com:ucsd-cse15l-s23/lab7.git <enter>`  
![Image](git-clone.png)  
3. Running the tests to see they fail: `bash test.sh <enter>`  
![Image](failedtests.png)  
4. Editing the code file: `43 j 11 l x i 2 <esc> : w q <enter>`  
![Image](edit-code.png)  
5. Running the tests to see they now succeed: `bash test.sh <enter>`  
![Image](successtests.png)  
6. Committing changes to fork: `git add ListExamples.java <enter>`, then `git commit -m "fixed test" <enter>`, then `git push origin main <enter>`  
![Image](gitaddcommit.png)  
![Image](gitpush.png)  
