# 0x1B. C - Sorting algorithms & Big O

## Introduction
This project focuses on implementing various sorting algorithms in C and understanding their time complexity using Big O notation. The project will be done in teams of two people, and the main objective is to gain a comprehensive understanding of sorting algorithms, their efficiency, and their applicability in different scenarios.

## Team Information
- Created by: Alexandre Gautier
- Done by: Mugambi Mungiria

## Project Timeline
- Start Date: June 21, 2023, 6:00 AM
- End Date: June 28, 2023, 6:00 AM
- Checker Release: June 23, 2023, 12:00 AM

## Background Context
Sorting algorithms are fundamental to computer science and play a vital role in efficiently organizing data. In this project, we will explore different sorting algorithms and their time complexities. Understanding Big O notation will help us evaluate the efficiency of algorithms and select the most appropriate one for a given input. Additionally, we will learn about stable sorting algorithms, which maintain the relative order of elements with equal values during sorting.

## Learning Objectives
By the end of this project, you should be able to:

- Implement at least four different sorting algorithms.
- Explain the concept of Big O notation and evaluate the time complexity of an algorithm.
- Select the best sorting algorithm based on the characteristics of the input data.
- Understand the concept of stable sorting algorithms.

## Requirements
### General
- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 20.04 LTS using gcc with the following options: `-Wall -Werror -Wextra -pedantic -std=gnu89`
- All your files should end with a new line
- A `README.md` file, placed at the root of the project folder, is mandatory.
- Your code should follow the Betty style. It will be checked using `betty-style.pl` and `betty-doc.pl`.
- Global variables are not allowed.
- Each source file should contain no more than 5 functions.
- The use of standard library functions like `printf`, `puts`, etc., is forbidden unless explicitly allowed.
- The project requires a header file named `sort.h` that contains the prototypes of all functions.
- All header files should have include guards.
- A list or array does not need to be sorted if its size is less than 2.

### GitHub
- Each team should have one project repository. Cloning, forking, or duplicating another project repository with the same name before the second deadline will result in a 0% score.

## Resources
Before starting the project, make sure to read or watch the following resources:

- Sorting algorithm
- Big O notation
- Sorting algorithms animations
- 15 sorting algorithms in 6 minutes (WARNING: The video contains visuals that can trigger seizures/epilepsy. It's not required for the project, but can be viewed for a visual representation of different sorting algorithms)
- CS50 Algorithms explanation in detail by David Malan
- All about sorting algorithms

## Data Structure and Functions
The project provides the following functions to print arrays and lists:

```c
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size)
{
    size_t i;

    i = 0;
    while (array && i < size)
    {
        if (i > 0)
            printf(", ");
        printf("%d", array[i]);
        ++i;
    }
    printf("\n");
}
```

```c
#include <stdio.h>
#include "sort.h"

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list)
{
    int i;

    i = 0;
    while (list)
    {
        if (i > 0)
            printf(", ");
        printf("%d", list->n);
        ++i;
        list = list->next;
    }
    printf("\n");
}
```

Your sorting functions will be compiled along with these files during evaluation. Make sure to declare the prototypes of print_array and print_list in your sort.h header file. For doubly linked lists, use the provided data structure:

```c
/**
 * struct listint_s - Doubly linked list node
 *
 * @n: Integer stored in the node
 * @prev: Pointer to the previous element of the list
 * @next: Pointer to the next element of the list
 */
typedef struct listint_s
{
    const int n;
    struct listint_s *prev;
    struct listint_s *next;
} listint_t;
```

Please note that this format is used for Quiz and Task questions.

## Copyright and Plagiarism
You are responsible for creating your own solutions to meet the learning objectives of this project. Copying and pasting someone else's work is strictly prohibited and will result in removal from the program. Do not publish any content related to this project.

## Testing
To test your sorting algorithms with large sets of random integers, you can use the following website: Random.org

## Big O Notation
When discussing the time complexity of algorithms, use the short notation for Big O. For example, O(nk) or O(wn) should be written as O(n). If an answer is required within a file, make sure to end the file with a newline.

## Conclusion
This project aims to enhance your understanding of sorting algorithms, Big O notation, and selecting appropriate sorting algorithms based on input data. By implementing different sorting algorithms and evaluating their efficiency, you will gain valuable insights into algorithmic complexity and improve your problem-solving skills. Remember to follow the project requirements, enjoy the learning process, and collaborate effectively with your team!

#### Please let me know if there's anything else I can help you with!
