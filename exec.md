# OS
System call
#we have 2 file c .the first ex1.c ,ex2.c ...
#ex1.c
#include <stdio.h>
#include<stdlib.h>
#include<unistd.h>

int main(int argc,char *argv[])
{
   printf("the pid of ex1.c is= %d \n",getpid());
   char *args[]={"Hello","os","world"};
   execv("./ex2",args);
   printf("we back");

    return 0;
}

**********
#now ex2.c
#include <stdio.h>
#include<stdlib.h>
#include<unistd.h>
int main(int argc,char *argv[])
{
    printf("I am in ex2.c \n");
    printf("the pid of ex2.c is= %d \n",getpid());
    return 0;
}
