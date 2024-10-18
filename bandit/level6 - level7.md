# Level 6 -> Level 7
In ths challenge we need to read a particular file that satisfies the given properties: it should be 33 bytes big, must be owned by the user bandit7 and the group bandit6.

# My Solve
Firstly I did `find -size 33c -group bandit6` thinking it would give me the file but as it is stored anywhere on the system i need to invoke the `find` command from the root directory so i did `cd /` then invoked the same command but now the problem was i was getting 2 files instead of one so i also put in the `user` aargument in the `find` command then i got my file. After that i simply read the file to get the password.
```bash
bandit6@bandit:~$ find -size 33c -group bandit6
bandit6@bandit:~$ find / -size 33c -group bandit6 2>/dev/null
/etc/bandit_pass/bandit6
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ find / -size 33c -group bandit6 -user bandit7 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:/$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
