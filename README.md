# README.md

This README file contains important Linux and GitHub commands that you should know.

## Table of Contents

- [GitHub](#github)
- [Git](#git)
- [Linux Commands](#linux-commands)

## GitHub

- **Creating a Repository**
 - To create a new repository on GitHub, go to your profile page and click on the green "New" button.

- **Cloning a Repository**
 - To clone a repository, open your terminal or command prompt and run the following command:
    ```
    git clone https://github.com/username/repository.git
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

## Git

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

- **Merging Branches**
 - To merge a branch into the master branch, first switch to the master branch and then run the following command:
    ```
    git merge branchname
    ```

- **Deleting a Branch**
 - To delete a branch, run the following command:
    ```
    git branch -d branchname
    ```

## Linux Commands

- **Creating a New Directory**
 - To create a new directory, run the following command:
    ```
    mkdir directoryname
    ```

- **Changing the Current Directory**
 - To change the current directory, run the following command:
    ```
    cd directoryname
    ```

- **Listing the Contents of a Directory**
 - To list the contents of a directory, run the following command:
    ```
    ls
    ```

- **Creating a New File**
 - To create a new file, run the following command:
    ```
    touch filename
    ```

- **Viewing the Contents of a File**
 - To view the contents of a file, run the following command:
    ```
    cat filename
    ```

- **Deleting a File or Directory**
 - To delete a file or directory, run the following command:
    ```
    rm -rf filename
    ```

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
