# lab-report-week-6
## Streamlining ssh Configuration
* .ssh/config file
![edit .ssh/config file](screenshot_week6/1_edit_config_file.png)
    How to edit the file: First, change directory to .ssh folder. Second, type "vim config". Third, press "i" to insert content, and press "esc" (keyboard) and ":wq" to quit editing. 
* Log into my account
![ssh_login](screenshot_week6/1_ssh_login.png)
    With the config file, I can enter my account on ieng6 with less typing.
* scp a file
![scp](screenshot_week6/1_scp_file.png)
    I can write "scp makefile ieng6:~/" instead of "scp makefile cs15lsp22amq@ieng6.ucsd.edu:~/"


## Setup Github Access from ieng6
* Public & Private key stored on my user account (ieng6)
![ieng6_server](screenshot_week6/2_ieng6_server_Public_private_key.png)
    Public and private keys are in .ssh folder. "id_rsa_github_pub" is the public key, and "id_rsa_github" is the private key.
* Public key stored on the Github.
![](screenshot_week6/2_Github_public_key.png)
add a new ssh key on Github
![](screenshot_week6/2_Github_public_key1.png)
The myMac_key is the ssh key of my computer, and the ieng6_key is the ssh key of my user account on ieng6.
* commit and push a change.
![](screenshot_week6/2_commit_push.png)
With ssh key, I don't need to type in username and password when we commit and push files.

## Copy whole directories with scp -r
* copy markdown-parse directory to ieng6 account.
![](screenshot_week6/3_copy_file.png)
    Copy all files with .md extension and files in the lib folder.
* Compile and run the test on ieng6 account
![](screenshot_week6/3_runfile.png)
* Copy and Run the test file in one line.
![](screenshot_week6/3_run_together.png)
Combine scp, ;, and ssh to copy the whole directory and run the tests in one line.