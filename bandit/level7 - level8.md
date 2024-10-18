# Level 7 -> Level 8
In this challenge the password is stored next to the word "millionth" in a file called `data.txt`.

# My Solve
FIrtsly i did `ls` to check if the file was indeed there. After that i used the `grep` command which finds a substring that we pass in as its parameter in a file that we specify. So doing `grep "millionth" data.txt` will search for the string that contains "millionth" in it in `data.txt`.
```bash
bandit7@bandit:~$ ls
data.txt
bandit7@bandit:~$ grep "millionth" data.txt
millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
