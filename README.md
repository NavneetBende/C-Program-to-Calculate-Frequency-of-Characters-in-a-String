Calculate Frequency of Characters
In this article we will learn how to code a C program to calculate frequency of characters in the string. Calculating frequency means to calculate how many times each character is present in a string. To calculate this we will use a for loop that will iterate each character of the string and then store the count of each of the characters in an array. Then we will use another for loop to print the frequency of each character that we have stored in an array.

Calculate Frequency of Characters in Cpp
Algorithm:
Initialize the variables.
Accept the input.
Initialize a for loop and terminate it at the end of string. 
This for loop will be used to count the number of time each character is present.
Initialize another for loop to print the frequency if it is at least 1.
While loop in C
C programming code to calculate the frequency of each character in a string
#include<stdio.h> 

int main()
{
    //Initializing variables.
    char str[100] ="prepinsta";
    int i;
    int freq[256] = {0};
    
    //Calculating frequency of each character.
    for(i = 0; str[i] != '\0'; i++)
    {
        freq[str[i]]++;
    }
    
    //Printing frequency of each character.
    for(i = 0; i < 256; i++)
    {
        if(freq[i] != 0)
        {
            printf("The frequency of %c is %d\n", i, freq[i]);
        }
    }
    return 0;
}
Output
The frequency of a is 1
The frequency of e is 1
The frequency of i is 1
The frequency of n is 1
The frequency of p is 2
The frequency of r is 1
The frequency of s is 1
The frequency of t is 1
