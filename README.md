# Core Concepts of Computer Programming 

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
Of all the inventions in the field of electronics 
like the radio and telephone, the programmable computer 
was the most significant one. It changed the
world forever.

If ever a certain device
can be programmed the way we want it to behave, then 
we can simply instruct it to do things for us.
That's very practical, isn't it?

After the programmable computers, the next
big question was how humans would program these computers.
They began developing programming languages and 
the 1970s was a very remarkable period: 
the C language was invented.

After the success, the great potential was unleashed
and we are now seeing the things a programmable computer
can do: the era of information, real-time data, 
almost realistic 3D games, artificial intelligence, etc.

Learning computer science now is a very sophisticated
one unlike it was in the past: there are too many 
fields even in software development alone.

And if you are a beginner, you might be discouraged
from all the things you need to learn but don't worry:
**you don't need to learn them all**. What you need
to learn first is the understanding how computers work
and the fundamentals of computer programming that
all computer programming languages have in common.

And since almost every programming language nowadays
directly and indirectly inherits concepts from 
the C language, we'll be using it to demonstrate
the core concepts of programming.

*Take note: we don't want to discuss every 
detail of the code in terms of the C language, 
rather we just want to get the core
concepts of computer programming that are
common in different programming languages.*

## Input And Output
As was mentioned, a programmable computer is very 
important but the way you interact with the computer
is through input and output: you as the user
will have an input, the computer will process it
(the way it is processed is programmed also),
then the computer will output something.
The very first demonstration is the "Hello World"
program. The programmer will tell the computer
to simply display the message on the screen.

But of course, complex programs are not as straightforward
as that. Typical programs like binary
to human language (and vice versa)
takes a lot of processing,
an operating system to recognize computer applications,
a business collaborative tool with a lot of features
to manage data, a 3D game that is almost realistic,
an Artificial Intelligence program that can simulate humans
in the virtual world!

But of all the things programmers can do, the 
computer only processes input as binary data
(0s and 1s) and 
it should not be interpreted literally. It's just
a representation of something a computer 
can recognize: absence or presence of electric pulse.
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

In this small program, the `#include`
tells the computer to include a certain
source which is needed because
it contains the predefined command `printf`.
`printf` simply tells the computer
to display the text provided by the programmer.

As simple as that, you have now the complete
idea of what a programmable computer is all about.
It's you telling the computer to do things it 
can handle in terms of binary data.

## Variables And Data Types
In computer programming, a **variable** is just like
a container to store digital data. A **data type**
is the way you tell the computer how that data
will be interpreted. Should the computer interpret
that as letters? or numbers? or words? or simply
raw binary data? The computer does not know 
that, you must tell it exactly.

In computer programming, both these things
will enable you to store data and tell 
the computer what kind of data it is. When you
store, you want to retrieve it later as per
needed. Remember also, computer's memory 
is different from storage. Think of it
as the short-term memory and the storage
(the hard disk) as the long-term memory.
But during the runtime of a program you 
are developing, you refer to memory as 
`storage`. The computer's memory has the full
access to the CPU while the disk does not have
that access.
In order to read contents from the hard disk,
a request should be made. Hence, in programming
you are using the memory first not the disk.
There is the current development to combine
the two but is still on-going.

Take note, the details of memory, hard disk
and CPU are quite complex but the mentioned
details above will serve as the starting point
for full comprehension.

### Sample Program for Variables and Data Types
```
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

In this simple program, we declare and assign 3
variables with different data types:
1. variable `i` that contains 1 numeric value
2. variable character `myletter[]`
that contains letters `myletter`
3. variable `x` that contains 1.23 value

After that, the program is telling the computer
to display these values.


## Operators
In programming just like in mathematics, there are 
operators and the most common in computer programming
are assignment, arithmetic and comparison operators.

### Assignment Operators Sample Program
```
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

The most common assignment operator is
`=` and it should not be confused with
the double `==` comparison operator.

This time, it is simply assigning a 
value to a variable. The result is:

```
c = 10
c = 15
c = 3
```

Variable `c` contains a value at a specific time.
It was changed in the program three times.

### Arithmetic Operators Sample Program
```
#include <stdio.h>

int main() {
    int a = 10;
    int b = 5;
    int result;

    printf("where a = %d & b = %d \n", a, b);

    result = a + b;
    printf("a+b = %d \n", result);
    result = a - b;
    printf("a-b = %d \n", result);
    result = a * b;
    printf("a*b = %d \n", result);
    result = a / b;
    printf("a/b = %d \n", result);

    return 0;
}
```
Since these are arithmetic operators, they
will do the basic arithmetic operations.

The result is:

```
where a = 10 & b = 5 
a+b = 15 
a-b = 5 
a*b = 50 
a/b = 2
```

### Comparison Operators Sample Program
```
#include <stdio.h>

int main() {
    int a = 10, b = 10, c = 20;

    printf("%d == %d is %d \n", a, b, a == b);
    printf("%d == %d is %d \n", a, c, a == c);
    printf("%d > %d is %d \n", a, b, a > b);

    return 0;
}
```
Since these are comparison operators, they are 
comparing the left and right side values.

The result is:

```
10 == 10 is 1 
10 == 20 is 0 
10 > 10 is 0 
```

The result is either 0 or 1 and remember,
0 is FALSE and 1 is TRUE.

## Conditionals
In a comprehensive program, the computer must decide
based on the condition/s given. Of course, the computer
cannot do that alone, you must instruct it exactly.
The most common is the
IF statement with the extended IF/ELSE.

### Sample Program Using IF
```
#include <stdio.h>

int main() {
    int i = 10;

    if (i == 10) printf("Expected value is the same as variable i, so the result is TRUE. \n");

    return 0;
}
```

In a single IF statement, the programmer wants to test,
expect or verify something, such as this program.
The programmer is expecting that `i` variable 
has the value 10, and variable `i` has the same 
value, so the statement 
`Expected value is the same as variable i, so the result is TRUE.`
will be printed. If the expected value is 
not the same as  the value of the variable, 
the statement will not be printed.

Sometimes, just an IF will not be sufficient,
particularly when you want to catch the FALSE result
or create a nested IF-ELSE. So, you want to extend it
and catch the FALSE result.

### Sample Program Using IF ELSE
```
#include <stdio.h>

int main() {
    int i = 10;

    if (i == 11) {
        printf("Expected value is the same as variable i, so the result is TRUE. \n");
    } else {
        printf("Expected value is not the same as variable i, so the result is FALSE. \n");
    }
    return 0;
}
```

Not only the statement in the ELSE branch will be printed,
you can do a lot of things just like correct an error,
go to a certain part of a program, etc. That's the power
of catching the FALSE result.

## Loops
There are commands or portions of your program
to be repeated several times. Loops are there to do
that. Now, there are simple loops and 
loops based on a given condition,
much like a repeated IF statement.
Simple loops are like repeat 10 times or repeat
forever. Conditional loops are loops with 
specific conditions other than simple iteration
just like in robot programming:
repeat until color red, repeat until the 
distance is less than 50mm, etc.

The most common that we see in computer
programming: the `for` loop,
`while` loop and `do-while` loop. 

### Sample Program Using Loops
```
#include <stdio.h>

int main() {

    int n = 11;

    int i;
    int x[n];
    printf("the `for` loop: \n");
    for (i = 1; i < n; i++) {

        printf("iteration: %d | Hello World. \n", i);
    }

    int y = 0;
    printf("------ \n");
    printf("the `while` loop: \n");
    while (y < 10) {
        y += 1;
        printf("iteration: %d | Hello World. \n", y);
    }

    y = 0;

    printf("------ \n");
    printf("the `do while` loop: \n");

    do {
        y += 1;
        printf("iteration: %d | Hello World. \n", y);
    }
    while (y < 10);

    return 0;

}
```

the result:
```
the `for` loop: 
iteration: 1 | Hello World. 
iteration: 2 | Hello World. 
iteration: 3 | Hello World. 
iteration: 4 | Hello World. 
iteration: 5 | Hello World. 
iteration: 6 | Hello World. 
iteration: 7 | Hello World. 
iteration: 8 | Hello World. 
iteration: 9 | Hello World. 
iteration: 10 | Hello World. 
------ 
the `while` loop: 
iteration: 1 | Hello World. 
iteration: 2 | Hello World. 
iteration: 3 | Hello World. 
iteration: 4 | Hello World. 
iteration: 5 | Hello World. 
iteration: 6 | Hello World. 
iteration: 7 | Hello World. 
iteration: 8 | Hello World. 
iteration: 9 | Hello World. 
iteration: 10 | Hello World. 
------ 
the `do while` loop: 
iteration: 1 | Hello World. 
iteration: 2 | Hello World. 
iteration: 3 | Hello World. 
iteration: 4 | Hello World. 
iteration: 5 | Hello World. 
iteration: 6 | Hello World. 
iteration: 7 | Hello World. 
iteration: 8 | Hello World. 
iteration: 9 | Hello World. 
iteration: 10 | Hello World.
```

As you can see here, it's just printing the 
Hello World ten times, whether it's `for` loop,
`while` loop or `do-while` loop.

## Functions
A function is a group of statements (commands)
that together perform a task.
There are built-in functions and functions that a 
programmer will create according to his/her needs.

### Sample Program Creating And Using Functions
```
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

The function `printFunctionTest()` is created by
declaring `void` first. Other functions will return values
but for the sake of simplicity we create a void `function`.
A `void` function will simply execute the commands
contained in it, nothing else.

Then inside the main function, you simply invoke it
by its name. And all the commands inside that function
will be executed line by line.

Why use functions? Imagine if there is none. Complex
programs are usually composed of thousands of lines of code
up to million, without any grouping, that will be
very hard to handle.

If a function is generic and can be used for other
projects, you can simply separate it for distribution.
So your code is now reusable.
