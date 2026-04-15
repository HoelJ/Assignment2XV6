# Assignment2XV6
This is the documentation for Assignment 2.\
All changed files will be in the following repository:\
https://github.com/HoelJ/Assignment2XV6\

I used nano to write to all necessary files:\
First, I added SYS_getprocs to syscall.h and assigned it the number 22.\
Then, I added SYS_getprocs to the syscalls[] array in syscall.c and made it point to sys_getprocs.\
After, in user/user.h, I added int getprocs(void);, while to user/usys.S, I put SYSCALL(getprocs).\
In sysproc.c, I wrote the function sys_getprocs(void) according to the directions.\
I created a program, getprocs.c, in the user directory by following the provided instructions. The file is attached to my submission.\
Below is the output after running my test:\
Input: $ getprocs \
Output: Processes running: 3
