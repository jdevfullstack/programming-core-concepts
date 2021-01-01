# Core Concepts of Computer Programming 
Of all the inventions in the field of electronics 
like radio and telephone, the programmable computer was the 
turning point for our modern world. It changed the
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

## Input / Output
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
an operation system to recognize computer applications,
a business collaborative tool with a lot of features
to manage data, a 3D game that is almost realistic,
an Artificial Intelligence that can simulate humans
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

int main()
{

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

## Variables & Data Types
In computer programming, a **variable** is just like
a container to store digital data. A **data type**
is the way you tell the computer how that data
will be interpreted. Should the computer interpret
that as letters? or numbers? or words? or simply
a raw binary data? The computer does not know 
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
access to the CPU while the disk does not have.
In order to read contents from the hard disk,
a request should be made. Hence, in programming
you are using the memory first not the disk.
There is the current development to combine
the two but it is still on-going.

Take note, the details of memory, hard disk
and CPU are quite complex but the mentioned
details above will serve as the starting point
for full comprehension.

### Sample Program for Variables and Data Types
```
#include <stdio.h>

int main()
{

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
are arithmetic, comparison, and assignment operators.

### Arithmetic Operators Sample Program
```
#include <stdio.h>
int main()
{
    int a = 10;
    int b = 5;
    int result;
    
    result = a + b;
    printf("a+b = %d \n", result);
    result = a - b;
    printf("a-b = %d \n", result);
    result = a * b;
    printf("a*b = %d \n", result);
    result = a / b;
    printf("a/b = %d \n", result);
    result = a % b;
    printf("Remainder when a divided by b = %d \n", result);
    
    return 0;
}
```

### Comparison Operators Sample Program
```
#include <stdio.h>
int main()
{
    int a = 10, b = 10, c = 20;

    printf("%d == %d is %d \n", a, b, a == b);
    printf("%d == %d is %d \n", a, c, a == c);
    printf("%d > %d is %d \n", a, b, a > b);

    return 0;
}
```


### Assignment Operators Sample Program
```
#include <stdio.h>
int main()
{
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

## Conditionals

## Loops

## Functions

## Structures


