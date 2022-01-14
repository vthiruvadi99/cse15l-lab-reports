# Lab Report 1 Week 2
## Downloading VScode
1. Go to the VSCode website to download the appropriate version of VScode: https://code.visualstudio.com/
![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/vscode%20download.png)
## Remotely Connecting
1. Open VScode and create a new file or import a java file
2. In the top menu bar click on terminal and then new terminal to see the terminal
3. In the terminal, use this command to input log in username information for the remote connection you are trying to make: ssh cs15lwi22zz@ieng6.ucsd.edu
This command will access the CSE computers on campus
4. The zz are replaced with the letters that are unique to your username and can be found through account lookup
5. Subsequently, you will be prompted for a password, and although the actual characters will not show while typing in the password the inputs are being stored
6. *I have been having trouble logging into my ssh and have contacted ITS and waiting for an escalation, I also posted on Piazza*
![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/sshloginattempt.png)
## Trying Some Commands
1. cd
2. cd~
3. ls -lat
4. ls -a
5. etc.
![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/linuxcommands.png)
## Moving Files With SCP
1. scp is used to copy files from one computer to a remote computer
2. The command looks like: scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/
3. the WhereAmI.java is a file that is in your local directory on your computer and the cs15lwi22zz@ieng6.ucsd.edu:~/ is the destination for the copy
4. ![image](![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/scp%20attempt.png)
## Settig An SSH Key
1. In order to avoid inputting your passowrd every time a ssh key can be used to conveniently access your account
2. using a program called ssh-keygen we can create a pair of files called public key and private key
3. by copying the public key to the server and the private key in a particular location the client then the simple ssh command will identify both keys and allow you in
![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/SSH%20Keys.png)
## Optimizing Remote Running
1. you can write commands in quotes at the end of an ssh command to directly run it on remote servers: ssh cs15lwi22@ieng6.ucsd.edu "ls"
2. semicolons can be used to run multiple commands on the same line: cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI
![image](https://github.com/vthiruvadi99/cse15l-lab-reports/blob/main/Screen%20Shot%202022-01-14%20at%203.46.33%20PM.png)
