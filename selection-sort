// Trying to code the different sort algorithms
#include <cs50.h>
#include <math.h>
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main(void)
{
    // Make sorted number array of size 50000
    int sorted_numbers[50000];
    // Fill the array with numbers
    for (int i = 0; i < 50000; i++)
    {
        sorted_numbers[i] = i + 1;
    }

    // Make reversed number array of size 50000
    int reversed_numbers[50000];
    // Fill the array with numbers
    for (int i = 49999; i >= 0; i--)
    {
        reversed_numbers[i] = 50000 - i;
    }

    // Make random number array of size 50000
    int random_numbers[50000];

    // Initialze boolean array of size 50000
    bool random_check[50000];
    // Set its contents to false
    for (int i = 0; i < 50000; i++)
    {
        random_check[i] = false;
    }

    // Initialize counter variable
    int random_index = 0;
    // Make sure numbers about to be generated are truly randomized on each execution
    srand(time(NULL));
    // Make while loop
    while (random_index < 50000)
    {
        // Generate random number between 1 and 50000
        int random_number = rand() % 50000 + 1;
        // If the random number is not in the random chek array yet
        if (random_check[random_number] == false)
        {
            // Add random number to random numbers array
            random_numbers[random_index] = random_number;
            // Mark it used in the random check array to avoid duplicates
            random_check[random_number] = true;
            // Move on to the next index
            random_index++;
        }
    }

    // TODO: Code selection sort
    for (int i = 0; i < 50000; i++)
    {
        int smallest_number = i;
        for (int j = i; j < 50000; j++)
        {
            if (random_numbers[j] < random_numbers[smallest_number])
            {
                smallest_number = random_numbers[j];
            }
        }
        
    }
    // TODO: Code bubble sort
    // TODO: Code merge sort
}
