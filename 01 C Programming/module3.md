### CHAPTER 1: ARRAYS

**Arrays**

Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

**Multidimensional Arrays**

Multidimensional arrays are arrays of arrays.

To create a two-dimensional array, add each array within its own set of curly braces

**Access the Elements of an Array**

You refer to an array element by referring to the index number

**Sorting Arrays**

- Sorting is the process of arranging data in a particular format.

- Types of Sorting:  
 **Bubble Sort**  
 **Selection Sort**  
 **Insertion Sort**  
 **Shell Sort**  
 **Merge Sort**  
 **Quick Sort**  

 **Searching Arrays**

- Searching is the process of finding an element within a list.

- Types of Searching:  
 **Linear Search**  
**Binary Search**  
 **Sequential Search**

 ### CHAPTER 2: STRING CONCEPTS

**Strings**  
A string is a sequence of characters

**String Variables and Literals**  
A string literal is a sequence of characters surrounded by double quotes
Character arrays are used to store strings
The only difference between array of char and string is that, a string must end with null character (\0)

**String Concatenation**

String concatenation is the process of joining two strings together

**String Length**

The length of a string is the number of characters it contains

**String Comparison**

String comparison is the process of comparing two strings to determine whether they are equal or not

**String Methods**  
String methods are built-in functions that can be used on strings.  
The following are some of the commonly used string methods:  

**charAt()**  - Returns the character at the specified index (position)  
**concat()**  - Joins two or more strings, and returns a new joined strings  
**indexOf()**  - Returns the position of the first found occurrence of a specified value in a string  
**lastIndexOf()**  - Returns the position of the last found occurrence of a specified value in a string  
**match()**  - Searches a string for a match against a regular expression, and returns the matches  
**replace()**  - Searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced  
**search()**  - Searches a string for a specified value, or regular expression, and returns the position of the match  
**slice()**  - Extracts a part of a string and returns a new string  
**split()**  - Splits a string into an array of substrings  
**substr()**  - Extracts the characters from a string, beginning at a specified start position, and through the specified number of character  
**substring()**  - Extracts the characters from a string, between two specified indices  
**toLowerCase()**  - Converts a string to lowercase letters  
**toUpperCase()**  - Converts a string to uppercase letters  
**toString()**  - Returns the value of a String object  
**trim()**  - Removes whitespace from both ends of a string  
**valueOf()**  - Returns the primitive value of a String object

```
char name1[] = “hello”;
char name2[10];
name2=name1; /* This initialization is invalid */
```
