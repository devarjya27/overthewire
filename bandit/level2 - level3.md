# Level 2 -> Level 3
In this challenge we need to read a file which has spaces in its name, To pass in the entire filename as the argument for `cat` we need to put double quotes around the filename otherwise it will only read the first word of the file name.
# My Solve
I put `spaces in this filename` under double quotes and passed it as an argument to `cat` to get the password.
```bash
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat "spaces in this filename"
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
