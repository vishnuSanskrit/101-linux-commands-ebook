# The `touch` Command.

Using `touch` Command A FILE argument that does not exist is created empty, unless -c or -h is supplied.

---
### Examples
1. To make a new text file use the following command, and if it does not already exist a new file will be created or overwritten otherwise.

```
touch file.txt

```
2. Touch command to create multiple files: Touch command can be used to create the multiple numbers of files at the same time. These files would be empty while creation.

```
touch File1_name File2_name File3_name 
```


---


#### **A  FILE  argument string of - is handled specially and causes touch to change the times of the file associated with standard output.**

#### Mandatory arguments to long options are mandatory for short options too.

1.   -a     
>change only the access time

2.  -c, --no-create
>do not create any files

3. -d, --date=STRING
>parse STRING and use it instead of current time

4. -f     
>(ignored)

5. -h, --no-dereference
>affect each symbolic link instead of any referenced file (useful  only  on  systems that can change the timestamps of a symlink)

6. -m     
>change only the modification time

7. -r, --reference=FILE
>use this file's times instead of current time

8. -t STAMP
>use [[CC]YY]MMDDhhmm[.ss] instead of current time

9. --time=WORD
>change  the specified time: WORD is access, atime, or use: equivalent to -a WORD is modify or mtime: equivalent to -m

10. --help 
>display this help and exit

11. --version
>output version information and exit



Note that the -d and -t options accept different time-date formats.
