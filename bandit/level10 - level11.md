# Level 10 -> Level 11
In this challenge the password is in a base64 encoded file.
# My Solve
As per the `base64` manpage if we pass `-d` as the argument for `base64` which stands for decode, the decoded output is printed to standard output.
```bash
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ base64 -d data.txt
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```
# Resources Used
`base64` manpage: <https://manpages.ubuntu.com/manpages/focal/en/man1/base64.1.html>
