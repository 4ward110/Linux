# Remove , Find, Edit, Moving, Copy, Sorting

## 1. Delete File and Folder
  
- Using `rm` command : you can find it by using `man rm` command
  
- `rm + path-to-file-need-to-delete...`ls

- To remove all file with same `tail` or `head` you can use `rm *.type-file-delete` or `rm head-all-file-need-delete*`

- To delete a folder use `rm -r folder-delete-name` with `-r` options mean `recursive`.

- `rmdir` can remove only empty directory

## 2. Copy file & folder
  
- to copy file using `cp` command.
  
- Copy a file to another file `cp file1 file2(file you want to parse content in file 1 to)`.
  
- Copy to a new destination `cp + file to copy + path`

- You can copy all files in a folder by using `*` to select all

- Copy a `folder` use `cp -r folder-to-copy + path`

## 3. Rename and moving
  
- Rename: Using `mv + old-file/folder-name + new-file/folder-name` command

- You can ussing `mv` command to move file or folder to another directory.

## 4. Locate (Searching)

- To use locate command you need to install `locate` & `mlocate` package from your repo.

- Example :`locate *.conf` => all path to .conf file

## 5. Find command

- Diff with `locate` and `find` command is locate need a db to work but find don't . find list all folder, file but `locate` list only file.

- Easy to read about find in manual

## 6. View file

- Using `cat` or `less` command to read file or `tac` to read file but from the bottom to top :)

- `rev` command can read but reverse each line ex hello => olleh :)

## 7. File Archiving and Compression

- `tar ball`: a way to putting your file to a bag to make them easier to compress and store. When you putting your file to a tar bar you store all your file in one place.

- 2 step to compress: 1/ make tarball 2/ compress tarball ussing some compress algorithms

- To put all file to a tarball using `tar -cvf <yournewfile>.tar file/folder-want-inside-tar` command.

- When you put your file in a tarball the size of tarball not equal the size of total files it's bigger than because the .tar file need space to store so you need give .tar memory.

- To extract a `.tar` file simply you use `tar -xvf <yourtarfile>.tar`.

- So how we compress the `tarball` smaller just use `bzip2` (slow than but more compression power) or `gzip` (faster but less compression power)

- Command: `gzip <your-tar-file>.tar` and to unzip `gunzip + <yourfile>.tar.gz`. same with `bzip2 <your-tar-file>.tar` & `bunzip <yourfile>.tar.bz2`

- To compress in 1 step you can use command : `tar -cvzf <compressfilename>.tar.gz <all file to compress>` or `tar -cvjf <compressfilename>.tar.bz2 <all file to compress>`

- And you can unzip a `gz` or `bz2` file by using `tar -xvzf <name>.tar.gz` or  `tar -xvjf <name>.tar.bz2`

- To create a `.zip` file you just 1 step `zip <your-file>` & `unzip`
