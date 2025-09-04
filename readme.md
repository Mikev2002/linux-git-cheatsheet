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
