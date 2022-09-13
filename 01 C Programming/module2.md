### CHAPTER 1: MANAGING INPUT AND OUTPUT OPERATIONS

**character**

The `getchar()` function reads a character from the standard input stream and returns it as an `int` value. The `getchar()` function is defined in the `stdio.h` header file.
```
char c = getchar();
```

**Ctypes.h**

The ctype.h header file is used to determine the type of a character. The functions are -

- isalpha()
- isdigit()
- isalnum()
- islower()
- isupper()
- isxdigit()
- isprint()
- isgraph()
- isblank()
- isspace()
- ispunct()
- iscntrl() 

**Write a character**

The `putchar()` function writes a character to the standard output stream. The `putchar()` function is defined in the `stdio.h` header file.

```
putchar(c);
```

**Formatted input/output**

The `printf()` function is used to write formatted output to the standard output stream. The `printf()` function is defined in the `stdio.h` header file.

```
printf("Hello, World!");
```

The `scanf()` function is used to read formatted input from the standard input stream. The `scanf()` function is defined in the `stdio.h` header file.

```
int a;
scanf("%d", &a);
```

**Rules for scanf/printf**

`Scanf`
- Each variable to be read must have a specification (address of proper type)
- Never end the format string with whitespace. It is a fatal error.
> The scanf will read until:  
> 1. A whitespace character is found in numeric specification.  
> 2. maximum number of characters have been read
> 3. An error is detected  
> 4. The end of file is reached  


`format codes`

Code | Meaning
---|---
%c | single character
%d | decimal integer
%e, %f, %g | floating point value
%h | short integer
%i | decimal integer
%o | octal integer
%s | string
%u | unsigned decimal integer
%x | hexadecimal integer
%[ ] | string of word

> The l can be used as a prefix for long integer. Ex: %ld

```
printf(“control string”, arg1, arg2, ..., argn);
```
Control string contains three types of items:
1. Characters that will be printed on the screen as they appear.
2. Format specifications that define the output format for display of each item.
3. Escape sequence characters such as \n, \t and \b.

```
printf(“a = %07d”, a); Rigth Align
printf(“a = % -7d”, a); Left Align

x=10.776;
printf(“%6.3f %”, x ); // 10.776

a=10, b=7777, c=88;
printf(“a=%4 b=%7d”, a , b); // a = __10 b = ___7777
```

**String input/output function**

- gets and puts are line oriented input output functions available in the `<stdio.h>`
header file.  
- gets( ): Alternative method to read strings
- puts( ): Alternative method to write strings

```
char name[10];
gets(name);

puts(name);
```

### CHAPTER 2: Decision Making and Branching

1. if statement
2. if – else statement
3. Nested if else statement
4. Cascaded if else

### CHAPTER 3: Decision Making and Looping

`Loop components`
1. Initialization (example: ctr=1, i=0 etc)
2. Test Condition (example: ctr<=500, i != 0 etc)
3. Updating loop control values (example: ctr=ctr+1, i =i-1)

**C language provides 3 looping structures**
1. while loop
2. do….while loop
3. for loop

```
int ctr=0, N=10;
while(ctr<=N) {
    printf(“Hello World\n”);
    ctr=ctr+1;
}
```

**break and continue**

- break statement is used to terminate the loop

- continue statement is used to skip the current iteration

