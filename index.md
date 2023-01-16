# Step 1: Installing VSCode

To Install VSCode, first navigate to the VSCode website, this can be accessed by typing in vscode into google.

![Image](https://jorryns.github.io/cse15l-lab-reports/week1vsc1.png)

Webpage

Click Download for Windows, or if you’re on mac Download for Mac probably.
Go Through the Installation Process.


# Step 2: Remotely Connecting

There are a couple parts to this step, first, you need to setup your password for your CSE15L course-specific account, install GIT if you're on windows, to do this follow this tutorial. 
https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit (course specific account)
To install GIT, you can find this on google as well. 

Next navigate to a new terminal on Visual Studio Code, if you are on Windows create a new bash terminal, by clicking the + above the terminal window.

In the bash terminal, type in "$ ssh cs15lwi23zz@ieng6.ucsd.edu" where zz is replaced by the letters in your course specific account

You will get a message saying the Authenticity of host cant be extablished, type in yes to continue and press enter.

Next it will ask you for a password, type in the password you set earlier in this step and log in.

You will get a message that says "Now on remote server"

![Image](https://jorryns.github.io/cse15l-lab-reports/week1ssh.png)

# Step 3: Running Commands

There are many commands that you can use both on your computer and the remote computer in order to highlight the differences.

For example cd~ 

On your computer it should bring you to here:

(Windows) C:\Users\user

But on the remote computer it should bring you to here:

"/home/linux/ieng6/cs15lwi23/cs15lwi2zz"

You can try next try cat /home/linux/ieng6/cs15lwi23/public/hello.txt in order to get this output:

"Hello! Welcome to CSE15L"

Heres a full list of specific useful commands to try:

![Image](https://jorryns.github.io/cse15l-lab-reports/week1commands.png)
