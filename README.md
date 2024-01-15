# README.md

This README file contains important Linux and GitHub commands that you should know.

## Table of Contents

- [GitHub](#github)
- [Git](#git)
- [VSCode](#VSCode)
- [Linux Commands](#linux-commands)
- [Bash Files](#Bash-Files)

## GitHub

- **Creating a Repository**
 - To create a new repository on GitHub, go to your profile page and click on the green "New" button.

- **set Git configuration**
 - To set up github on the local git, open your terminal or command prompt and run the following commands:
    ```
    git config --global user.name “-------”
    git config --global user.email “------”
    ```

- **set Git configuration**
 - To check your github configuration on the local git, run the following commands:
    ```
    git config --list
    ```

- **Cloning a Repository**
 - To clone a repository, open your terminal or command prompt and run the following command:
    ```
    git clone git@github.com:username/repository.git
    ```
    
- **connect to a remote repository on GitHub**
 - Run this git command to connect your local Git repository to a remote repository on GitHub.
   ```bash
    git remote add origin git@github.com:username/repositoryname.git
   ```
   
- **Adding a File to the Repository**
 - To add a file to the repository, first make sure the file is in the correct directory. Then, open your terminal or command prompt and navigate to the directory where the file is located. Finally, run the following command:
    ```
    git add filename
    ```

- **Commiting Changes**
 - After adding the file, you can commit the changes to the repository with the following command:
    ```
    git commit -m "commit message"
    ```

- **Pushing Changes to GitHub**
 - To push the changes to the GitHub repository, run the following command:
    ```
    git push origin master
    ```
    
- **Update your repo to the latest changes**
 -  If you already have a local copy of the repository and you want to update it, you can use the git pull command. This command fetches changes from the remote repository and merges them into your local branch.
    ```
    git pull origin main
    ```
    ```
    git pull git@github.com:username/repository.git master
    ```
    
## Git

- **Initializing a new repository**
 - To create a new repository
    ```
    git init
    ```
    
- **Creating a New Branch**
 - To create a new branch, run the following command:
    ```
    git checkout -b branchname
    ```

- **Switching Between Branches**
 - To switch between branches, run the following command:
    ```
    git checkout branchname
    ```
    
- **current status of your working directory**
 - This command shows you which files have been modified, staged, or deleted and the brach you are currently on. Additionally, it will show you any conflicts that may have arisen during a merge or rebase.
    ```
    git status
    ```
    
- **Merging Branches**
 - To merge a branch into the master branch, first switch to the master branch and then run the following command:
    ```
    git merge branchname
    ```
    ```
    git merge branchname --no-edit -m "commit message"
    ```

- **Deleting a Branch**
 - To delete a branch, run the following command:
    ```
    git branch -d branchname
    ```
    
- **view the commit history**
 - This will display a list of all the commits made to the repository, including the author, date, and commit message.
    ```
    git log
    ```
    
## VSCode

- **Open VSCode using terminal**
 - To open VSCode simply write:
    ```
    code
    ```
    
- **Open a file using VSCode**
 - To open a file using VSCode simply write:
    ```
    code [filename]
    ```
    
## Linux Commands
- **printing working directory**
 - To print the path of the working directory, starting from the root
   ```
   pwd
   ```
- **Creating a New Directory**
 - To create a new directory, run the following command:
    ```
    mkdir [directoryname]
    ```

- **Changing the Current Directory**
 - To change the current directory, run the following command:
    ```
    cd [directoryname]
    ```
 - To change the current directory to parent directory, run the following command:
    ```
    cd ..
    ```
 - To change the current directory to root directory, run the following command:
    ```
    cd .
    ```
- **Listing the Contents of a Directory**
 - To list the contents of a directory, run the following command:
    ```
    ls
    ```

- **Creating a New File**
 - To create a new file, run the following command:
    ```
    touch [filename]
    ```
    
- **editing the file**
 - To open and edit a file, run the following command:
    ```
    vi [filename]
    ```
    
- **Disk uusage**
 - To analyze and report on disk usage within directories and files.
    ```
    du [directory/file]
    ```
    
- **Viewing the Contents of a File**
 - To view the contents of a file, run the following command:
    ```
    cat [filename]
    ```

- **Deleting a File or Directory**
 - To delete a file or directory, run the following command:
    ```
    rm -rf [filename]
    ```
- **history of executed command**
 - To view previously executed commands:
    ```
    history
    ``` 
- **Generate a new SSH key pair**
 - This following command will generate a new SSH key pair. It creates a RSA key pair and saves the private key to a file named "id_rsa" in the "~/.ssh" directory, and it saves the public key to a file named "id_rsa.pub" in the same directory.
   ```bash
   ssh-keygen -t rsa
   ```
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
 - This command will generate a new SSH key pair. It creates a 4096-bit RSA key pair and saves the private key to a file named "id_rsa" in the "~/.ssh" directory, and it saves the public key to a file named "id_rsa.pub" in the same directory. The -C flag is used to add a comment, which is useful for identification purposes.
   
- **Searching for a File or Directory**
 - To search for a file or directory, run the following command:
    ```
    find / -name "filename" 2>/dev/null
    ```

- **Downloading a File**
 - To download a file, run the following command:
    ```
    wget fileurl
    ```

- **Extracting a Zip File**
 - To extract a zip file, run the following command:
    ```
    unzip filename.zip
    ```

- **Compressing a Directory**
 - To compress a directory into a zip file, run the following command:
    ```
    zip -r filename.zip directoryname
    ```

- **Moving a File or Directory**
 - To move a file or directory, run the following command:
    ```
    mv filename destination
    ```

- **Renaming a File or Directory**
 - To rename a file or directory, run the following command:
    ```
    mv oldfilename newfilename
    ```

- **Updating the System**
 - To update the system, run the following command:
    ```
    sudo apt-get update && sudo apt-get upgrade
    ```

- **Checking the System's Uptime**
 - To check the system's uptime, run the following command:
    ```
    uptime
    ```
    
## Bash Files
- **To create a bash script file with the .sh extension. For example, my_script.sh.**
 - Add a shebang line at the beginning of the script to specify the interpreter. In this case, we will use bash.
    ```bash
    #!/user/bin/bash
    ```
 - Write your script commands under the shebang line. Each command should be on a new line. For example, let's print "Hello, World!" and list the files in the current directory.
    ```bash
    #!/user/bin/bash

    echo "Hello, World!"

    ls
    ```
 - Save your script file.

 - Open a terminal and navigate to the directory where your script file is located.

 - Give the script file execute permissions by running the following command:

    ```bash
    chmod +x my_script.sh
    ```
 - Now you can run your script by executing the following command:

    ```bash
    ./my_script.sh
    ```
 - This will execute your script and display the output in your terminal.

 - Remember to replace my_script.sh with the actual name of your script file.
 - EXAMPLE:
   ```bash
   #!/user/bin/bash
   greeting = "welcome"
   user = $(whoami)
   day = $(date + %A)
   echo "greeting back $user! Today is $day, which is the best day of the entire week!"
   echo "your bash shell version is $BASH_VERSION. Enjoy!"
   ```
