# Week 1 Lab Report
Within CSE 15L we are required to install vscode and remote into ieng6. These are a summary of how to set up remote connection and various commands to make the connection easier to use. 

This tutorial makes the assumption that you are using an OSX operating system, meaning that SSH is already available to you out of the box.

[Install VS Code](#vscode)

[Remote Connection](#remote)

[Trying Some Commands](#commands)

### <a name="vscode">
# Installing VS Code
</a>
The IDE used for this setup is Microsoft's Visual Studio Code. The download link can be found here:

![Image](screenshots/week1/vscodeinstall.png)

[Download Visual Studio Code](https://code.visualstudio.com/)

Follow the steps until VS code is properly installed on your system.


### <a name="remote">
# Remote Connection</a>

In order to connect to ieng6 remote servers, prerequisite steps have to be fulfilled.

- Make sure ieng6 account is properly updated with a password.
- if it is not updated log into this website to [change password](https://sdacs.ucsd.edu/~icc/index.php)

Once the passwords have been set up, open VScode and create a new terminal.

 - To log into your account first type in `ssh` then your account@ieng6.ucsd.edu, in my case it is `ssh cs15lfa22hs@ieng6.ucsd.edu`
 -  It will now prompt you for a password. Enter your password.

 - In the chance that this does not work, use your regular username as the username e.g. `ssh jbuensuceso@ieng6.ucsd.edu` and use your AD password.

 After successful login, your terminal should look like this:

![Image](screenshots/week1/terminalremote.png)

Congratulations you are now sucessfully connected to the ieng6 server.

### <a name="commands">
# Trying Some Commands</a>

Once connected to the terminal, try using the `ls` command.

![Image](screenshots/week1/ls.png)

As you can see, it shows the contents of the current directory.

Another command is: `cat /home/linux/ieng6/cs15lfa22/public/hello.txt`

![Image](screenshots/week1/cat.png)

This command concatenates the file, in this case, `hello.txt` and prints out the contents

