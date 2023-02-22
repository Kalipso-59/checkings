#include "get_next_line.h"
#include <stdio.h>
#include <time.h>

int main(void)
{
    clock_t start, end;
double execution_time;
start = clock();


    int fd = open("file.txt", O_RDONLY);
    char *line;

    while ((line = get_next_line(fd)) != NULL)
    {
        printf("%s\n", line);
        free(line);
    }

    close(fd);
    
end = clock();
execution_time = ((double)(end - start))/CLOCKS_PER_SEC;
printf("\nruntime : %f", execution_time);
    return 0;
}

