## LAB 10

**The following program defines a function that takes an integer and returns its square. It then uses a loop to call the function ten times, printing out the squares of the first ten numbers.**
```
 #include <stdio.h>

     int square(int n)
     {
          return n*n;
     }

     int main()
     {
          int i;

          for (i = 0; i<10; i++)
          {
              printf("The square of %d is %d\n", i, square(i));
          }
          return 0;
     }

```

**Make a copy of this program as prog1.c; compile it and make sure it works.**
**Change the program so that as well as printing out the squares of each number, it now prints out the cubes as well. You should write a function to calculate the cube of a number and use this in your answer.**

**Complete the following program, prog2.c, by defining the function toUpper() which**

**takes one parameter c of type char**
**returns a result of type char which is**
**the upper case equivalent of c if it is a lower case letter**
**the value of c otherwise**

```
     #include <stdio.h>

     char toUpper(char c)
     {
          /*  complete the definition of function toUpper() here */
     }

     int main()
     {
          char input[256];
          int i;

          printf("Input a string of characters: "); scanf("%[^\n]%*c", input);

          for (i=0; input[i] != '\0'; i++)
          {
                   printf("%c",toUpper(input[i]));
          }
          printf("\n");
          return 0;
     }

```

**Compile prog2 and test that it works correctly.**

**Write a program,prog3.c which**

**defines a function called isFactor( ) which**
**takes two integer parameters m and n**
**returns true (1) if m divides exactly into n and false (0) otherwise.**
**defines a main( ) function which**
**reads in two numbers from the user**
**uses the function isFactor( ) to check if the first input number divides exactly **into the second input number.**
**If the answer is true, the program should print an appropriate message and then read in two more numbers and repeat the whole process. The program should keep on looping like this while the first input number divides exactly into the second.**
**If the answer is false, the program should print an appropriate message and halt.**
