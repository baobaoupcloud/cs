---
title : "Conditionals"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---
Conditionals are constructs that perform different actions depending on the conditions. 


For example we can give conditions for the program to do comparison:
1. In the terminal window, type `code compare.c` and write code as follow:
```bash
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int x = get_int("What's x? ");
    int y = get_int("What's y? ");

if (x < y)
    {
        printf("x is less than y\n");
    }
elseif (x > y)
    {
        printf("x is greater than y\n");
    }
else{
        printf("x is equal to y\n");
    }
}
```
We created 2 variables type integer x, y. The values of these are populated using the get_int function. The first `if` clause checks whether the condition is satisfied, the function returns the corresponding value. If the condition is not met, the logic then evaluates subsequent conditions of `elseif` clause. Finally, if none of the previous conditions are fulfilled, it returns the `else` value.

2. Run the code by executing `make compare` in the terminal window, followed by `./compare`.
3. Input the 2 numbers and get the results.

The process of the program can be shown as **flow charts**. Such charts can be used to examine the efficiency of our code.

Following is the flow chart of the above code:
![flowchart](https://raw.githubusercontent.com/baobaoupcloud/cs-w1/main/static/images/4.conditionals/1conditionals.png)

