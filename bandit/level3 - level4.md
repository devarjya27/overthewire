# Level 3 -> Level 4
In this challenge we need to read a hidden file, we know that doing `ls -a` will list all the files even if they are hidden. Once we find the name of the file we can read it through `cat`.

# My Solve
Firstly I did `cd inhere` to change my directory to `inhere` after that i did `ls -a` to view the hidden file. After that passing `...Hiding-From-You` as the argument for `cat` allowed me to read the file and gave me the password.
```bash
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere
bandit3@bandit:~/inhere$ ls -a
.  ..  ...Hiding-From-You
bandit3@bandit:~/inhere$ cat "...Hiding-From-You"
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
