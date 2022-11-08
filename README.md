# simple_shell
Creating our own linux shell
Your shell will be compiled this way:gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

shell should work like this in interactive mode:
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$

 non-interactive mode:
 $ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
