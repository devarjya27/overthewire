# Level 8 -> Level 9
In this challenge we need to find the password which occurs only once in `data.txt`.

# My Solve
After reading the manuals for `uniq` i found out that using `-u` as the argument for `uniq` suppresses all the text that repeats, and to use this command we need to first use `sort`  to sort the text alphabetically as `uniq` only compares the adjacent lines of text. So after sorting we `pipe` the output and then invoke `uniq -u` so that it displays the text that appears only once.
```bash
bandit8@bandit:~$ sort data.txt | uniq -u
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```
# Resources Used
`uniq` manpage: <https://manpages.ubuntu.com/manpages/focal/en/man1/uniq.1posix.html>

`sort` manpage: <https://manpages.ubuntu.com/manpages/focal/en/man1/sort.1.html>
