# FIND-THE-SUM-OF-DIGITS
Find the sum of digits of a number using recursion

#include <stdio.h>
 

int sum_of_digit(int n)
{
    if (n == 0)
       return 0;
    return (n % 10 + sum_of_digit(n / 10));
}
 

int main()
{
    int num = 78965;
    int result = sum_of_digit(num);
    printf("Sum of digits in %d is %d\n", num, result);
    return 0;
}

============================================================================

OUTPUT

-------------------------------

Sum of digits in 78965 is 35
