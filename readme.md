# Linux & Git Command Cheat SHeet

### ls
The `ls` command lists the files and directories in the current directory.

***Example:***
```
ls -l
```

### cd
The `cd` command changes the current working directory

***Example:***
```
cd
```

### pwd 
The `pwd` command prints the current workiing directory ( the folder you are in).

***Example:***
```
pwd
```

### mkdir
The `mkdir` command creates a new directory (folder).

***Example:***
```
mkdir projects
```
***Create nested folders (create parents as needed):***
```
mkdir -p projects/src
```

### touch
The `touch` command creates an empty file or updates the timestamp of an existing file

***Example:***
```
touch notes.txt
```
```
touch notes1.txt notes2.txt
```

### rm
The `rm` command removes files. Use `-r` to remove directories recursively. `-i` asks for confirmation (safer).

***Example:***
```
rm notes.txt
rm -r projects/
rm -ri projects/ #interactive, prompts before each removal
```

### mv
The `mv` command moves or renames files and directories.

***Example:***
```
mv old name.txt newname.txt         #rename a file
mv notes.txt docs/                  #move a file into directory
mv file1.txt file2.txt docs/        #move multiple files
mv -i report.txt docs/              #prompt before overwrite
mv -n report.txt docs/              #do not overwrite existing files
mv -v *.txt docs/                   #verbose: show what moved
```

### cp
The `cp` command copies files and driectories.

***Example:***
```
cp notes.txt backup/            # copy a file into a directory
cp file1.txt file2.txt docs/    # copy multiple files
cp -r src/ project-backup/      # copy a directory recursively
cp -i report.txt backup/        # prompt before overwrite
cp -n report.txt backup/        # never overwrite existing files
cp -v *.md docs/                # verbose:show what's copied
```

### cat
The `cat` command displays the contents of files or concatenates them.

***Examples:***
```
cat notes.txt                               # view a file
cat file1.txt file2.txt > combined.txt      # combine into a new file
cat -n script.sh                            # show line numbers
```

### grep
The `grep` command searches for lines matching a pattern in files.

***Examples:***
```
grep "error" app.log                # basic search
grep -i "error" app.log             # case-insensitive
grep -n "main()" *.c                # show line numbers
grep -r "TODO" src/                 # recursive search in a folder
grep -E "cat|dog" animals.txt       #extemded regex (OR)
grep -v "^#" config.ini             # invert match (exclude commented lines)
```

### head
The `head` command shows the first lines of a file (10 lines by default).

***Examples:***
```
head notes.txt
head -n 20 notes.txt
```

### git status
Shows the state of the working directory and staging area (which files are untracked, moditfied, or staged).

***Example:***
```
git status
```
### git add
Stages changes so they'll be included in the next commit.

***Examples:***
```
git add readme.md # stage one file
git add. # stage everything in the current directory
git add -p # interactively choose hunks to stage
```


