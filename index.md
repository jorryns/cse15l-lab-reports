# Step 1: Installing VSCode

To Install VSCode, first navigate to the VSCode website, this can be accessed by typing in vscode into google or follow the link here.
Webpage: [VSCode](https://code.visualstudio.com/)

![Image](https://jorryns.github.io/cse15l-lab-reports/week1vsc1.png)

Image of the Webpage.


Click Download for Windows, or if you’re on mac Download for Mac.
Navigate to the installation folder, and run the installer.
Follow the installer directions (this should only take a minute).
It should now be installed under: C:\Users\{Username}\AppData\Local\Programs\Microsoft VS Code




# Step 2: Remotely Connecting

There are a couple parts to this step, first, you need to setup your password for your CSE15L course-specific account, install GIT if you're on windows, to do this follow this tutorial. 
[doc](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit) (course specific account)
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

cd stands for change directory and it changes the working directory of the terminal. The ~ means home directory so it should bring your working directory of the terminal to the root directory of your computer.

On your computer it should bring you to here:

```
(Windows) C:\Users\user
(Mac) User\~
```

But on the remote computer it should bring you to here:

```
"/home/linux/ieng6/cs15lwi23/cs15lwi2zz"
```

This is the home directory of the remote computer because it is the root directory of the user you are currently login as.

You can try next try cat /home/linux/ieng6/cs15lwi23/public/hello.txt in order to get this output:

"Hello! Welcome to CSE15L"

Heres a full list of specific useful commands to try:

![Image](https://jorryns.github.io/cse15l-lab-reports/week1commands.png)
