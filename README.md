PRINTING PATTERN:
      *

    ***

  *****

*******

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r. The loop should be structured as for( i=0 ; i<r : i++).
 Run a nested loop inside the main loop to print the spaces before the pyramid. From k=r to k>i +1. The loop should be structured as for( k=r; k>i+1 ;k–).
Inside this nested loop print white space.
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=0 to j<=i*2. The loop should be structured as for( j=0 ; j<i*2; j++).
Inside this nested loop print star.
Move to the next line by printing a new line . printf(“/n”).
Code in C:
#include<stdio.h>
int main()
{
int i,j,k,r;     //declaring integer variables i,j,k for loops and r for number of rows
printf("Enter the number of rows :\n");     //Asking user for input
scanf("%d",&r);      //saving number of rows in variable r
for(i=0;i<r;i++)    //outer loop for number of rows
   {
     for(k=r;k>i+1;k--)     //nested loop for number of spaces
       {
          printf(" ");     //printing spaces
       }
     for(j=0;j<=i*2;j++)     //nested loop for printing stars
       {
          printf("*");      //printing stars
       } 
    printf("\n");     //printing newline
   }
}
TAKING INPUT:
DISPLAYING OUTPUT:
