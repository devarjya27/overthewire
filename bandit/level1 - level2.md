# Level 1 -> Level 2
Here we need to read a file named `-` located in the home directory. Simply doing `cat -` doesnt work as `-` is interpreted as stdin/stdout and `cat -` takes input from us alllowing us to pass data to the command.
# My Solve
To tackle this problem, I did `cat ./-` which means go to my current working directory and read a file named `-`.
```bash
bandit1@bandit:~$ ls
-
bandit1@bandit:~$ cat -
^C
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
