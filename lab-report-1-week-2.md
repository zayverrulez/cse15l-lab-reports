# Week 2 Lab Report

## Installing VSCode

To start, we downloaded Visual Studio Code at the following website URL: 
https://code.visualstudio.com/

Then we followed the instructions to install it on our computers.

After a relatively quick and painless set-up here is what things look like:

*Photo of installed VSCode*

![Image](/Screenshot_1.png)



## Remotely Connecting

Firstly, OpenSSH has to be installed on my computer:
https://sdacs.ucsd.edu/~icc/index.php

Following this guide: https://code.visualstudio.com/docs/remote/ssh#_connect-to-a-remote-host

I opened up the terminal, typed in:

`ssh `

then I added my specific account username.

`cs15lsp22auw@ieng6.ucsd.edu`

Finally, once prompted, I typed in my password. Once connected the computer listed the System stats.

System Stats:

    * Last Login
    * Quota
    * 0% of CPU
    * Cluster Status
    * Prepping

*Picture of this interaction and system stats*

![Image](/Screenshot_2.png)

## Trying Some Commands

My group and I made an effort to try every command listed in the lab and lecture notes. These commands allow you view and or modify files on the remote computer.

*Here are some of the commands that my group mates and I tried out:*

![Image](/Screenshot_3.png)

## Moving Files with scp

We used the following command to move files over SSH to the remote computer:

`scp`

Using the created test file named `WhereAmI.java` I issued the following command to copy the file over:

`scp WhereAmI.java cs15lsp22auw@ieng6.ucsd.edu`

Then I was prompted to put in a password. After which the copy was complete. Finally, to prove the copy worked, I tested the file by compiling and running it.

*An image of a success scp file copy onto the remote computer.*

![Image](/Screenshot_4.png)

![Image](/Screenshot_7.png)

## Setting an SSH Key

To start, on my client computer I typed:

`ssh-keygen`

To which the computer responded:

```
Generating public/private rsa key pair.

Enter file in which to save the key

(/Users/<user-name>/.ssh/id_rsa):
```

To which I entered:


`/Users/Xavie/.ssh/id_rsa`

To which the computer responded:


`Enter passphrase (empty for no passphrase):`

I did not add a paraphrase as instructed.

Then I logined into the SSH remote computer and issued the following command to make a folder for the ssh files:

`mkdir .ssh`

Then I logged out. Back on my client I used an scp copy file command to move the ssh key files to the ssh folder on the remote computer:

`scp /Users/Xavie/.ssh/id_rsa.pub cs15lsp22auw@ieng6.ucsd.edu:~/.ssh/authorized_keys`

*Now the ssh connection does not need a password as demonstrated in this picture:*

![Image](/Screenshot_5.png)

## Optimizing Remote Running

Remote running can be simplified by not having to login in to execute a command. For example, if you add the command you wish to run through ssh in quotes at the end of a ssh connect command, the command will just be ran without having to log out.

`ssh cs15lsp22auw@ieng6.ucsd.edu "ls"`

And you can also add multiple commands in one line by adding a ";"

`cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI`

Using the up-arrow to recall the last command ran, my team mates and I came up with ideas for the simplist/least involved usage of typing/commands. 

*Here are a few ideas my group members and I came up with.*
 
![Image](/Screenshot_6.png)