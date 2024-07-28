# Core Concepts of Computer Programming 

*`updated 28 May 2023`*

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fjdevstatic%2Fprogramming-core-concepts&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=PAGE+VIEWS&edge_flat=false)](https://hits.seeyoufarm.com)

TOC
1. [Intro](#intro)
2. [Input / Output](#input-and-output)
    1. [Hello World Program](#hello-world-program)
3. [Variables & Data Types](#variables-and-data-types)
    1. [Sample Program for Variables and Data Types](#sample-program-for-variables-and-data-types)
4. [Operators](#operators)
    1. [Assignment Operators Sample Program](#assignment-operators-sample-program)
    2. [Arithmetic Operators Sample Program](#arithmetic-operators-sample-program)
    3. [Comparison Operators Sample Program](#comparison-operators-sample-program)
5. [Conditionals](#conditionals)
    1. [Sample Program Using IF](#sample-program-using-if)
    2. [Sample Program Using IF/ELSE](#sample-program-using-if-else)
6. [Functions](#functions)
    1. [Sample Program Creating And Using Functions](#sample-program-creating-and-using-functions)

## Intro
Of all the inventions in the field of electronics like the radio and 
telephone, the programmable computer was the most significant one. It 
changed the world forever.

If a certain device can be programmed the way we want it to behave, 
then we can simply instruct it to do things for us. That's very 
practical, isn't it?

After programmable computers, the next big question was how humans 
would program them. They began developing programming languages and 
the 1970s was a very remarkable period: the C language was invented.

After this success, great potential was unleashed, and we are now 
seeing what a programmable computer can do: the era of information, 
real-time data, almost realistic 3D games, artificial intelligence, 
etc.

Learning computer science today involves many specialized fields, 
unlike in the past: there are many fields even in software development 
alone.

And if you are a beginner, you might be discouraged from all the things 
you need to learn but don't worry: **you don't need to learn them all**. 
What you need to learn first is understanding how computers work and 
the fundamentals of computer programming that all computer programming 
languages have in common.

And since almost every programming language nowadays directly and 
indirectly inherits concepts from the C language, we'll be using it to 
demonstrate the core concepts of programming.

*Take note: we don't want to discuss every detail of the code in terms 
of the C language, rather we just want to get the core concepts of 
computer programming that are common in different programming 
languages.*

## Input And Output
As was mentioned, a programmable computer is very 
important, but the way you interact with the computer
is through input and output: you, as the user,
will provide input, the computer will process it
(the way it is processed is also programmed),
then the computer will output something.
The very first demonstration is the "Hello World"
program. The programmer will tell the computer
to simply display the message on the screen.

But of course, complex programs are not as straightforward
as that. Typical programs like binary
to human language (and vice versa)
takes a lot of processing,
an operating system to recognize computer applications,
a business collaborative tool with many features
to manage data, a 3D game that is almost realistic,
an Artificial Intelligence program that can simulate humans
in the virtual world!

But of all the things programmers can do, the 
computer only processes input as binary data
(0s and 1s), and it should not be interpreted literally.
It's just a representation of something a computer 
can recognize: the absence or presence of an electric pulse.
Compare this with any drawing 
that can be accomplished just
by simply using a dot-and-no-dot pattern!
It's the same thing for the computer.

### Hello World Program

```
#include <stdio.h>

int main() {

    printf("Hello World!\n");
    printf("Life is a blessing!\n");

    return 0;

}
```

In this small program, the `#include` tells the computer to include a 
certain source which is needed because it contains the predefined 
command `printf`. `printf` simply tells the computer to display the 
text provided by the programmer.

As simple as that, you now have the complete idea of what a 
programmable computer is all about. It's you telling the computer to 
do things it can handle in terms of binary data.

## Variables And Data Types

In computer programming, a **variable** is just like a container to 
store digital data. A **data type** is the way you tell the computer 
how that data will be interpreted. Should the computer interpret that 
as letters? or numbers? or words? or simply raw binary data? The 
computer does not know that, you must tell it exactly.

In computer programming, both these things will enable you to store 
data and tell the computer what kind of data it is. When you store, 
you want to retrieve it later as needed. Remember also, computer's 
memory is different from storage. Think of it as the short-term memory 
and the storage (the hard disk) as the long-term memory. But during 
the runtime of a program you are developing, you refer to memory as 
`storage`. The computer's memory has full access to the CPU while the 
disk does not have that access. In order to read contents from the 
hard disk, a request should be made. Hence, in programming, you are 
using the memory first, not the disk. There is current development to 
combine the two, but it is still ongoing.

Take note, the details of memory, hard disk, and CPU are quite complex, 
but the mentioned details above will serve as the starting point for 
full comprehension.

### Sample Program for Variables and Data Types
```c
#include <stdio.h>

int main() {

    int i = 1;
    char myletter[] = "myletter";
    float x = 1.23;

    printf("int i: %d\n", i);
    printf("char myletter[]: %s\n", myletter);
    printf("float x: %f\n", x);

    return 0;
}
```

In this simple program, we declare and assign 
three variables with different data types:
1. an integer variable `i` that contains the numeric value `1`
2. a character array `myletter[]` that contains the string `"myletter"`
3. a float variable `x` that contains the value `1.23`

After that, the program instructs the computer to display these values.

## Operators
In programming, just like in mathematics, there are operators. The most 
common in computer programming are assignment, arithmetic, and 
comparison operators.

### Assignment Operators Sample Program
```c
#include <stdio.h>

int main() {
    int c;

    c = 10;
    printf("c = %d\n", c);
    c = 15;
    printf("c = %d\n", c);
    c = 3;
    printf("c = %d\n", c);

    return 0;
}
```

The most common assignment operator is `=`. It should not be confused 
with the double `==` comparison operator.

In this example, the `=` operator is simply assigning a value to a 
variable. The result is:

```
c = 10
c = 15
c = 3
```

Variable `c` contains a value at a specific time. It was changed in the 
program three times.

### Arithmetic Operators Sample Program
```c
#include <stdio.h>

int main() {
    int a = 10;
    int b = 5;
    int result;

    printf("where a = %d & b = %d\n", a, b);

    result = a + b;
    printf("a + b = %d\n", result);
    result = a - b;
    printf("a - b = %d\n", result);
    result = a * b;
    printf("a * b = %d\n", result);
    result = a / b;
    printf("a / b = %d\n", result);

    return 0;
}
```

Since these are arithmetic operators, they will perform basic arithmetic operations.

The result is:

```
where a = 10 & b = 5
a + b = 15
a - b = 5
a * b = 50
a / b = 2
```

### Comparison Operators Sample Program
```c
#include <stdio.h>

int main() {
    int a = 10, b = 10, c = 20;

    printf("%d == %d is %d\n", a, b, a == b);
    printf("%d == %d is %d\n", a, c, a == c);
    printf("%d > %d is %d\n", a, b, a > b);

    return 0;
}
```
Since these are comparison operators, they compare the left and right side values.

The result is:

```
10 == 10 is 1
10 == 20 is 0
10 > 10 is 0
```

The result is either 0 or 1. Remember, 0 is FALSE and 1 is TRUE.

## Conditionals
In a comprehensive program, the computer must make decisions based on given 
conditions. Of course, the computer cannot do this alone; you must instruct it 
exactly. The most common conditional statement is the `IF` statement, often 
extended with `IF/ELSE`.

### Sample Program Using IF
```c
#include <stdio.h>

int main() {
    int i = 10;

    if (i == 10) {
        printf("Expected value is the same as variable i, so the result is TRUE.\n");
    }

    return 0;
}
```

In a single `IF` statement, the programmer wants to test, expect, or verify 
something. In this program, the programmer expects that the variable `i` has 
the value 10. Since variable `i` does have the value 10, the statement 
`Expected value is the same as variable i, so the result is TRUE.` will be 
printed. If the expected value is not the same as the value of the variable, 
the statement will not be printed.

Sometimes, just an `IF` statement is not sufficient, particularly when you want 
to handle the FALSE result or create a nested `IF-ELSE`. In such cases, you 
extend it to catch the FALSE result.

### Sample Program Using IF ELSE
```c
#include <stdio.h>

int main() {
    int i = 10;

    if (i == 11) {
        printf("Expected value is the same as variable i, so the result is TRUE.\n");
    } else {
        printf("Expected value is not the same as variable i, so the result is FALSE.\n");
    }

    return 0;
}
```

Not only can the statement in the `ELSE` branch be printed, but you can also 
perform various actions such as correcting an error, navigating to a certain 
part of a program, etc. That's the power of catching the FALSE result.

## Loops
There are commands or portions of your program to be repeated several times. 
Loops are there to do that. Now, there are simple loops and loops based on a 
given condition, much like a repeated IF statement. Simple loops are like 
"repeat 10 times" or "repeat forever." Conditional loops are loops with 
specific conditions other than simple iteration, just like in robot 
programming: "repeat until color red," "repeat until the distance is less than 
50mm," etc.

The most common loops that we see in computer programming are the `for` loop, 
`while` loop, and `do-while` loop.

### Sample Program Using Loops
```c
#include <stdio.h>

int main() {
    int n = 11;
    int i;
    int x[n];

    printf("The `for` loop:\n");
    for (i = 1; i < n; i++) {
        printf("Iteration: %d | Hello World.\n", i);
    }

    int y = 0;
    printf("------\n");
    printf("The `while` loop:\n");
    while (y < 10) {
        y += 1;
        printf("Iteration: %d | Hello World.\n", y);
    }

    y = 0;
    printf("------\n");
    printf("The `do-while` loop:\n");
    do {
        y += 1;
        printf("Iteration: %d | Hello World.\n", y);
    } while (y < 10);

    return 0;
}
```

The result:
```
The `for` loop:
Iteration: 1 | Hello World.
Iteration: 2 | Hello World.
Iteration: 3 | Hello World.
Iteration: 4 | Hello World.
Iteration: 5 | Hello World.
Iteration: 6 | Hello World.
Iteration: 7 | Hello World.
Iteration: 8 | Hello World.
Iteration: 9 | Hello World.
Iteration: 10 | Hello World.
------
The `while` loop:
Iteration: 1 | Hello World.
Iteration: 2 | Hello World.
Iteration: 3 | Hello World.
Iteration: 4 | Hello World.
Iteration: 5 | Hello World.
Iteration: 6 | Hello World.
Iteration: 7 | Hello World.
Iteration: 8 | Hello World.
Iteration: 9 | Hello World.
Iteration: 10 | Hello World.
------
The `do-while` loop:
Iteration: 1 | Hello World.
Iteration: 2 | Hello World.
Iteration: 3 | Hello World.
Iteration: 4 | Hello World.
Iteration: 5 | Hello World.
Iteration: 6 | Hello World.
Iteration: 7 | Hello World.
Iteration: 8 | Hello World.
Iteration: 9 | Hello World.
Iteration: 10 | Hello World.
```

As you can see here, it's just printing "Hello World" ten times, whether it's 
a `for` loop, `while` loop, or `do-while` loop.

## Functions
A function is a group of statements (commands) that together perform a task. 
There are built-in functions and functions that a programmer will create 
according to his/her needs.

### Sample Program Creating And Using Functions
```c
#include <stdio.h>

void myFunction() {
    printf("Hello World.\n");
    printf("Life is beautiful.\n");
    printf("Cherish every single moment.\n");
}

int main() {
    myFunction();
    return 0;
}
```

The function `myFunction()` is created by declaring `void` first. Other 
functions will return values, but for simplicity, we create a void function. 
A `void` function will simply execute the commands contained in it, nothing 
else.

Then inside the main function, you simply invoke it by its name. All the 
commands inside that function will be executed line by line.

Why use functions? Imagine if there were none. Complex programs are usually 
composed of thousands to millions of lines of code. Without any grouping, 
that would be very hard to handle.

If a function is generic and can be used for other projects, you can simply 
separate it for distribution. So your code is now reusable.

## More Of My Content
- [jdevfullstack Profile](https://github.com/jdevfullstack)
- [jdevfullstack Repos](https://github.com/jdevfullstack?tab=repositories)
- [jdevfullstack Projects](https://github.com/jdevfullstack-projects)
- [jdevfullstack Tutorials](https://github.com/jdevfullstack-tutorials)
