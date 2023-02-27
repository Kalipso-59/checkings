# checkings

notes :)  ( flags for check correctness ( -Wall -Wextra -Werror -fsanitize=address -fno-omit-frame-pointer )
*********************************************************************************************************************************************************
AAB
{
       
       A-accept
       A-adapt
       B-become better
}

FAIL-First Attempt In Learning

* don't worry it's OK ;)

*********************************************************************************************************************************************************
GNL_PROJECT 

{
      
      1.gnl checking via command line:

             cc -Wall -Wextra -Werror -D BUFFER_SIZE=42 <files>.c

      2. check with testers 

      3. check manually.. I usually do it in online gdb.

      4. use my main
}

{


#include "get_next_line.h"
#include <stdio.h>

int main()
{
    int fd = open("input.txt", O_RDONLY);
    char *line = get_next_line(fd);
    while (line)
    {
        printf("%s\n", line);
        free(line);
        line = get_next_line(fd);
    }
    close(fd);
    return 0;
}
}
********************************************************************************************************************************************************

PRINTF_PROJECT

{
     
      1. check with tester (tripouelle, maybe)
 
      2. check with my main manually
 
}

********************************************************************************************************************************************************

BORN2BEROOT

{
}
