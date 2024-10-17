# Level 5 -> Level 6
In this challenge, we are given certain specifications for the file. The file must be 1033 bytes big, must be not executable and must be human readable. So finding the right parameters for the commands will help us get the password
# My Solve
As the file size is given as 1033 bytes, I found that if we pass `1033` as the parameter for the argument `-size` of the `find` command we get the file that has the password in it. I also found that if the size is in bytes, I need to follow up the size with a `c` when we pass the size as a parameter for the `size` argument.
After that i simply read the file using `cat`.
```bash
bandit5@bandit:~$ ls
inhere
bandit5@bandit:~$ cd inhere
bandit5@bandit:~/inhere$ find -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
