# lab-report-1-week-2

Tutor about how to log into a course-specific account on ieng6.

1. you need to install Visual Studio Code (or use a terminal on your computer, they are basically the same).
![Installing_VScode](screenshot_week2/Installing_VScode.png)

2. look up your course-specific account for CSE15L in [UCSD_Website](https://sdacs.ucsd.edu/~icc/index.php)

3. open a terminal and type in ssh cs15lsp22zz@ieng6.ucsd.edu. (replace zz with the letters in your course-specific account.)
![Remotely_Connecting](screenshot_week2/Remotely_Connecting.png)

    If you see something like the picture above, congratulations, you are login in successfully!

You can try some command.
* cd ~
* cd
* ls -lat
* ls -a
![Trying_Some_Commands](screenshot_week2/Trying_Some_Commands.png)

Using _command scp_ to copy a file from my computer to a remote computer.

![Moving_Files_with_scp](screenshot_week2/Moving_Files_with_scp.png)
* Compile and run the java file from _the server_.
![RunJava_on_the_server](screenshot_week2/RunJava_on_the_server.png)
* Compile and run the java file from _the client_.
![Run_file_on_the_client_computer](screenshot_week2/Run_file_on_the_client_computer.png)

We can establish a ssh key to avoid typing (or copy-paste) our password while connecting to the server.

1. Using ssh-keygen to generate _public and private key_.
2. Enter the file in which to save the key.
3. Go to the server, and copy the _public key_ to the .ssh folder.
![Setting_an_SSH_Key](screenshot_week2/Setting_an_SSH_Key.png)

After using the public and private keys, I can log in/scp files easier without using a password!
![Optimizing_Remote_Running](screenshot_week2/Optimizing_Remote_Running.png)
