# Fibonacci-series-
//C program code for Fibonacci series | Using recursion method 

    #include <stdio.h>

    int fib(int a);

    int main()
    {
        int a;
        int i;

        printf("Enter the number\n");
        scanf("%d", &a);

        for (i = 1; i <= a; i++)
        {
            printf("%d\n", fib(i));
        }
      return 0;
    }

    int fib(int a)
    {
        if (a == 1)
        {
            return 0;
        }
        else if(a == 2)
        {
            return 1;
        }
        else
        {
            return fib(a - 1) + fib(a - 2);
        }
    }
