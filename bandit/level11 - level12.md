# Level 11 -> Level 12
In this challenge, the password is encrypted using ROT13, a encryption technique where all letters have been rotated by 13 characters.
# My Solve
We know that the `tr` command helps in translating characters. Its usage is of the form `tr string1 string2`, input characters  found  in  string1  are  mapped  into  the corresponding  characters of string2.
And we know that the shifting is done by 13 characters so A maps to N and Z maps to M and such is the case with their lowercase counterparts also thus we can decode the encryption using `tr 'A-Za-z' 'N-ZA-Mn-za-m'`. Piping the output of `cat data.txt` to the input of `tr` will give us the required decrypted output.
```bash
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```

# Resources Used
`tr` manpage: <https://manpages.ubuntu.com/manpages/focal/en/man1/tr.1plan9.html>
