# Level 4 -> Level 5
In this challenge we look for a human-readable file in the `inhere` directory. As we know for a file name that starts with `-` we change the directory to the directory of the file and we invooke it using its relative path, thats what i did.
# My Solve
```bash
bandit4@bandit:~$ ls
inhere
bandit4@bandit:~$ cd inhere
bandit4@bandit:~/inhere$ ls
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09
bandit4@bandit:~/inhere$ cat ./-file00
�p��&�y�,�(jo�.at�:uf�^���@bandit4@bandit:~/inhere$ cat ./-file01
i�R�,�Λ�:Y���?�%�A����B��ͩ�bandit4@bandit:~/inhere$ cat ./-file02
3�	�)Ʈ�#Y��-6c��IR-�$����:��bandit4@bandit:~/inhere$ cat ./-file03
���/�
     ������qGi��,�2�Yb�
dbandit4@bandit:~/inhere$ cat ./-file04
�rOx����h0~ey
��c�~�h�n��G1bandit4@bandit:~/inhere$ cat ./-file05
}���ߓ��ߤ��W>��#lk�d�ܮ��yE��bandit4@bandit:~/inhere$ cat ./-file06
6�0]�\�$�1�%�������o@��b/��bandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
