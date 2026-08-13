# Reverse-a-Five-Digit-Number-in-C
This program takes a five‑digit number as input. 
It extracts each digit using modulus and division operations. 
Finally, it reconstructs the digits in reverse order and displays the result.


#include <stdio.h>
int main()
{
    long num, d1, d2, d3, d4, d5, reverse;
     // Prompt user to enter a five-digit number
     
    printf("Enter a five digit number: ");
    scanf("%ld", &num);
// Extract digits one by one from the end

    d1 = num % 10;   num = num / 10;
     d2 = num % 10;   num = num / 10;
    d3 = num % 10;   num = num / 10;
    d4 = num % 10;   num = num / 10;
     d5 = num % 10;   num = num / 10;
    
 // Reconstruct the number in reverse order 
 
 reverse = d1 * 10000 + d2 * 1000 + d3 * 100 + d4 * 10 + d5;
 
 // Display the reversed number
 
    printf("Reverse of the number is: %ld", reverse);
    
    return 0;  
    }
