# ~Week 2 Lab Report ~ 



## Installing VScode
 To install Visual Studio Code, head over to [VS Code](https://code.visualstudio.com/) and install the correct version for your current operating system. 
 ![image](https://user-images.githubusercontent.com/97643301/149487660-69592e37-6e38-4f27-8f0a-8bff40289fc6.png)

Once installed, run Visual Studio Code and you should have a similar-looking program as the image:
![image](https://user-images.githubusercontent.com/97643301/149488043-ffb8e672-381c-477f-975a-8ce59c77c8ef.png)

## Remotely Connecting
In order to remote connect, you need your own person account provided by UCSD. To retrieve this account, head to [Account Lookup](https://sdacs.ucsd.edu/~icc/index.php). Follow the steps provided by logging in with your UCSD account info, and proceed to retrieve the CSE 15L Course specific account. 

The page to retrieve your account should look like this: ![image](https://user-images.githubusercontent.com/97643301/149488927-f6f6e38e-c8cb-40a3-b5bb-60d0cb71d60c.png)

**NOTE:** Your CSE 15L account should look similar to this: `cse15lwi22alg@ieng6.ucsd.edu` where the alg is different and specified for your own unique 3 letters.

Once you retrieve your account, keep note of it and open VS Code. Open a terminal in VS Code by pressing Terminal on the top and pressing New Terminal. 

 A terminal on the bottom of VS Code should appear like so: ![image](https://user-images.githubusercontent.com/97643301/149489426-6eea0e17-9def-4887-bb58-297cff895b72.png)

**NOTE:** Your default terminal will show your user, and not the user in the image.

We will then use the `ssh` command which allows us to connect to the remote desktop at UCSD.
Type in the terminal `ssh cs15lwi22___@ieng6.ucsd.edu` where the ___ is your specified letters for your unique account. If you are logging in for the first time, it will ask `Are you sure you want to continue connecting (yes/no/[fingerprint])?` At this point type in yes and press enter. It then should continue to prompt your to enter your password. Enter the password that you assigned to to your account when you first retrieved it through the UCSD's Account Lookup. 

**IMPORTANT NOTE**: Your password will not be showed being typed in the terminal, however even though you can't see it, it is still taking the input given through your keyboard. An easy way to ensure your password is being inputted correctly, you can copy and paste your password into the terminal.

Once you log in, you should have a similar looking terminal:
![image](https://user-images.githubusercontent.com/97643301/149490453-e4a43fcb-06dd-4688-b38e-c5162b4f16de.png)

## Trying Some Commands
At this point you can try using some different commands! Try different commands within the SSH remote desktop and on your local client and noting the different outputs that are given through each one! 
Here are some commands:
- `ls` lists files in current directory
- `ls -l` lists all files in the current directory plus additional info such as last edited 
- `ls -a` lists all files including hidden files in the current directory
- `ls -lat` lists all files including hidden files in current directory and provides additional info
- `pwd` gives absolute path of directory
- `cd` takes you back to the home directory
- `mkdir` creates a new folder
- `rmdir` removes a directory
- `scp` copies a file onto a server
- `open` opens a file 
- `touch` creates a new file
- `rm` removes a file
- `du` gets the size of files and folders in a directory

Here are some commands being used on my client!: ![image](https://user-images.githubusercontent.com/97643301/149491804-aca43c0c-80bd-4839-a5ca-cdad072aaef5.png)

## Moving Files with scp
To move files from your local client to the ssh remote computer, the command `scp` is used. 
Type in your terminal `scp SomeFile.filetype cs15lwi22___@ieng6.ucsd.edu:~/` 
 
 **NOTE:** The `:~/` must be included following your account in order for it to be moved to your ssh remote computer.
 
Once the command is inputted, it will prompt you to enter your password in order to send the file over.

![image](https://user-images.githubusercontent.com/97643301/149492669-a56cd700-5a74-4650-b456-c4b0498d6f78.png)

## Setting an SSH Key
An SSH Key is used to create a pairing with your local client with your ssh remote computer where you no longer have to input your password whenever you use the ssh or scp command.

In order to create an SSH key, use the command `ssh-keygen` on your terminal.
![image](https://user-images.githubusercontent.com/97643301/149493119-f0e34d5f-d8f3-4fda-9c81-932654098ab6.png)

It will then prompt you where you want to save the file. By pressing Enter without typing anything in, it will create it within your current directory. If you would like you could type in a directory in which you would like the SSH key to be saved.

It will continue to ask you to input a password for the key. You can leave this empty by just pressing enter, or you can input your own password.
Then it will continue to ask your for your password for a second time. If you left it empty, just press enter, if not type in your password that you created.

You should then receive where the identification and public key were saved, your key fingerprint, and the key's random image. Should look like:
![image](https://user-images.githubusercontent.com/97643301/149493866-83bdcefb-b9d8-4a12-99fa-3c3b2917ccd8.png)

Keep note of your directory for your public rsa key which should look like `/Users/Username/.ssh/id_rsa.pub`

Then SSH back onto your remote computer, and use the command `mkdir .ssh` in order to create a directory for your public rsa key.

Then back on your local client use the command `scp /Users/Username/.ssh/id_rsa.pub cs15lwi22___@ieng6.ucsd.edu:~/.ssh/authorized_keys`

### YOU ARE NOW ABLE TO SSH AND SCP WITHOUT USING A PASSWORD
## Optimizing Remote Running
In order to do things faster and optimizing remote running, a method that is used is typing all the commands in one-go in the terminal separated by `;`.
For example you can do `touch SomeTxt.txt; scp SomeTxt.txt cs15lwi22___@ieng6.ucsd.edu:~/; ssh cs15lwi22____@ieng6.ucsd.edu; ls` and it will run the commands inputted it in consecutive order.

Another you can do that would save a lot of time is creating an alias and running that alias that contains all the commands you need to run. For example `alias test="scp whereami.java cs15lwi22alg@ieng6.ucsd.edu:~/; ssh cs15lwi22alr@ieng6.ucsd.edu 'javac whereami.java';ssh cs15lwi22alg@ieng6.ucsd.edu 'java WhereAmI'". ` 
This initially takes more than 10 key strokes, however once the alias is created, all you have to do is type in test in the terminal and it will run through the commands given which only takes **5** key strokes, and you can rename test to be a shorter word that will allow you to type it in less key strokes!

