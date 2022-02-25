# Streamlining SSH Configuration
My .ssh folder is on my desktop, where I could also find the config file as well.
<img width="592" alt="image" src="https://user-images.githubusercontent.com/97643301/153520003-d0b753bf-6975-4e9f-b6dd-e05e4d6a8bcd.png">

In order to access the contents of the config file, I use my computer's native app "TextEdit" as a way to edit the contents of the file.
<img width="156" alt="Screen Shot 2022-02-10 at 4 33 41 PM" src="https://user-images.githubusercontent.com/97643301/153520228-49f65a2f-df00-4c18-90eb-f532f77e132a.png">

By using my computer's native app "TextEdit" I add the following text in order to streamline my SSH and adding the following to the config file. 

**NOTE: You can change the name after `Host` to any name you would like, as this will be the name you type after typing `ssh`.**
```
 Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lwi22zzz (use your username)
```

**NOTE: May have to add the following line after user if `ssh` doesn't work. `IdentityFile ~/.ssh/id_rsa_ucsd`**
<img width="678" alt="Screen Shot 2022-02-10 at 4 36 27 PM" src="https://user-images.githubusercontent.com/97643301/153520744-e17f0331-80d1-4543-a632-156629b7beb4.png">

I can now `ssh` on the terminal by using the name I inputted after `Host`, in this case for me I chose ieng6!
<img width="446" alt="Screen Shot 2022-02-10 at 4 43 01 PM" src="https://user-images.githubusercontent.com/97643301/153521243-3bd6c6c0-9ade-4605-9fb8-79fbc58d00ae.png">

To see how much faster things are, I can also use other commands such as `scp` using the name I chose (ieng6) instead of having to type my entire UCSD ieng6 account name!

<img width="1137" alt="image" src="https://user-images.githubusercontent.com/97643301/155792668-2087f8d9-712f-4fcb-a42f-36b51cd4a995.png">


<img width="446" alt="Screen Shot 2022-02-10 at 4 43 01 PM" src="https://user-images.githubusercontent.com/97643301/153521398-a641446f-dc42-4be7-84ff-7ae81157d340.png">

Voila! And it's there!

<img width="836" alt="image" src="https://user-images.githubusercontent.com/97643301/153521459-77b83454-4129-4104-9391-9281cb2c2b7b.png">



