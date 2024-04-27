# LINUX COMMANDS

1. [Common](#common)


## Common
- **lsof -i tcp:8070** - find process which uses port 
- **kill -3 or -15 or -9 \<PID>** - kill process\
    3 - quit\
    15 - terminate\
    9 - kill

 - **cat** {filename} - view a file\
    -n - shows line number
 - **less** {filename} - shows end of file
 - **ahead** {filename} - shows head of file
 - **tail** {filename} - shows end of file
    -50 - number of lines\
    -f - real time
 - **mv** {filename} {filename1} - renames file
 - **touch** {filename} - creates file
 - **rm** {filename} - removes file
 - **cp** {file} {newFile} - makes file copy 
    -r {folder} {newFolder} - makes new folder recursive
 - **find** . -name {file} - finds files
    -iname - ignores case of file name
    - type\
        -d - directory\
        -f - file
 - **ls -l** - shows rules of security
    **-rw-rw-r--**;   **-rw-** - owner; **rw-** - members group; **r--** - others members
 - **chmod** - changes rules of security\
   -R - recursive\
    u - owner\
    g - member group\
    o - others\
    a - all users\
    0 - None\
    1 - only execute\
    2 - only write\
    3 - write/execute\
    4 - only read\
    5 - read/execute\
    6 - read/write\
 - **pwd** - prints directory
 - **ls** - shows folder content
 - **cd ..** - folder back
 - **cd -** -shows last operation
 - **cd ~** - returns to root
- **tar**
  -zcvf archive.tar.gz /path/to/files - to zip
  -zxvf archive.tar.gz -C / - to unaip
