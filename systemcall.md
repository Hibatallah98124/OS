# OS
System call
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
