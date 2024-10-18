# Level 9 -> Level 10
In this challenge the password is located in `data.txt` and is a human readable string preceded by many `=`.

# My Solve
To find human readable strings in a file we need to use the `strings` command and its also given that the password is preceeded by many `=` so we use `grep` command to search for a sequence of `=`. Thus what we need to do is pipe the output of `strings data.txt` which gives all the human readable strings to the `grep` command and then searches for `==` and thus we get our password.
```bash
bandit9@bandit:~$ ls
data.txt
bandit9@bandit:~$ strings data.txt | grep "=="
}========== the
3JprD========== passwordi
~fDV3========== is
D9========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```
# Resources Used
`strings` manpage: <https://manpages.ubuntu.com/manpages/focal/en/man1/strings.1plan9.html>
