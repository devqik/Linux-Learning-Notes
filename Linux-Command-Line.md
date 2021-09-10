# Linux Command Line


# 1- Command Structure

Command - Options - Arguments

`ls -a /var/log`


</br>


- ls -> Will list the contents of the current directory

- ls -l -> Will list the contents of the current directory with long listing option, that will list more details like owner of the document, permissions, date of last change

</br>

# 2- Useful keyboard shortcuts

</br>

- **Tab** : Will auto compelete the directory

- **Press Tab 2 times** : If there are multiple directories with the identical first letters, double tab will give you al list of suggestions. Also if you just remember the first letters of a command double tab will give you suggestions for commands to use.

- **Ctrl + A**: Move the cursor to the begining of the line

- **Ctrl + E** : Move the cursor to the end of the line

- **Ctrl + Left arrow**: Moves the cursor one word to the left

- **Ctrl + Right arrow**: Moves the cursor one word to the right

- **Ctrl + U** : Remove (Crop) characters from the cursor to the start

- **Ctrl + K** : Remove (Crop) characters from the cursor to the end

- **Ctrl + Y**: Paste croped text

- **Ctrl + Shift + C** : Copy text to the clipboard

- **Ctrl + Shift + V** : Paste text from the clipboard

- **Ctrl + R** : Search command history

- **Ctrl + C** : Cancel command


</br>

# 3- Find More Info About Commands

</br>

**1- Manual pages**

man ls -> Will give you information about the ls command and all the options and arguments used with it.

**2- Help option**

ls --help -> Gives information about the command but sometimes will refer you to the manual pages for more info


</br>

# 4- Files, Folders and Permissions

</br>

## Basics Of Dealing With Folders

</br>

- **file myfile.txt** -> Determine the type of the file

- **stat myfile.txt** -> Display ownership, modification information , etc ...

- **cd** -> Change directory

- **pwd** -> Print working directory

- **cd sample\ project** -> the back slash is used to escape the special characters and make bash know that it is a part of the directory name and not a second argument

- **ls -R** -> List the contents of a folder recursively, meaning that it will also list the contents of each sub-folder

- **cd ..** -> The .. represents the parent directory of the current directory

- **cd -** -> Will take you to the previously used directory

- **cd** -> Will take you to your home directory


</br>

## Create And Remove Folders

</br>

- **mkdir new_folder** -> Will create a new folder inside the current work directory

- **mkdir hello_world/new_folder** -> Will create a new folder inside the sub folder hello_world

- **mkdir hello_world1 hello_world2 hello_world3** -> mkdir can create multiple folders at once

- **mkdir -p hello_word/devops/project** -> Will create the parent folders hello_world and devops if they are not created yet

- **rmdir hello_world** -> Removes the folder hello_world , but it has to be empty to be removed

</br>

## Copy, Move And Delete FIles

</br>

- **cp devops.txt devops2.txt** -> Will copy the devops.txt file to a new file called devops2.txt

- **cp devops.txt project/pipeline/** -> Will copy the file devops.txt to the project/pipeline folder

- **mv devops.txt project/pipeline** -> Will move the devops.txt file to the desired folder

- **mv devops.txt project/pipeline/script.txt** -> Will move the devops.txt file to the desired directory and rename it to script.txt

- **mv \*.txt project/pipeline** -> Move every file with its name containing .txt in the end to the desired directory

- **mv project/pipeline/\* .** -> Move everything in the folder project/pipeline to the current working directory

- **rm devops?.txt** -> If you have files called devops1.txt, devops2.txt, devops3.txt ... etc, this command will delete all the files with the name devops followed by 1 charachter .txt

- **rm -r project** -> Will delete the contents of project folder recursively


</br>

## Search For Files

- **find . -name "devops\*"**-> Search for a file or directory with devops in its name followed by any charachters

- **find . -name "*.txt"** -> Will search for any file with .txt at the end of its name

- **find . -name "*d*"** -> Will search for any file or directory with letter "d" in its name


</br>

# 5- Super User

- **sudo** -> Will give you super user permissions

- **sudo -k** -> Will exit super user mode

- **sudo -s** -> Will make you access the root user

- **exit** -> Type exit to return from the root user to your normal user


</br>

