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
Type in the terminal `ssh cs15lwi22___@ieng6.ucsd.edu` where the ___ is your specified letters for your unique account. It should continue to prompt your to enter your password. Enter the password that you assigned to to your account when you first retrieved it through the UCSD's Account Lookup. 

**IMPORTANT NOTE**: Your password will not be showed being typed in the terminal, however even though you can't see it, it is still taking the input given through your keyboard. An easy way to ensure your password is being inputted correctly, you can copy and paste your password into the terminal.

Once you log in, you should have a similar looking terminal:
![image](https://user-images.githubusercontent.com/97643301/149490453-e4a43fcb-06dd-4688-b38e-c5162b4f16de.png)

 
 
## Trying Some Commands
## Moving Files with scp
## Setting an SSH Key
## Optimizing Remote Running
