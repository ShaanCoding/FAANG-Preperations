# Introduction to Data Structure - Arrays 101

## Introduction

- Arrays are simple data structures for storing similar items. They all exists in programming languages
- In this explore card we'll introduce arrays and store show them

- We're showing what:
  - What an array is
  - Basic properties of arrays
  - Implementing basic array operations
  - Simple programming techniques with arrays

### What is an array?

> An array is a collection of items. The items could be integers, strings, DVDs, game, book - anything really. The items are stored in neighboring (contigous memory) locations. Because they're stored together, checking through the entire collection of items straightforward.

### Creating an array

- On a computer, arrays can hold up to `N` items. This value is decided by you

```java
int[] integerArray = new int[5];
```

### Writing to an Array

- To put a DVD into the array, we need to decide which of the 15 places we'd like for it to go in. The identified number is 0 to `N-1`

```java
integerArray[3] = "value";
```

### Reading Items from an array

```java
System.out.println(integerArray[3]);
```

### Writing items into an array with a loop

```java
int[] squareNumbers = new int[10]
for(int i = 0; i < 10; i++) {
    int square = (i + 1) * (i + 1);
    squareNumbers[i] = square;
}
```

### Reading items from an array with a loop

```java
for(int i = 0; i < 10; i++)
{
    System.out.println(squareNumbers[i]);
}

for(int square : squareNumbers) {
    System.out.println(square);
}
```

### Array Capacity

- Lets say we create a array like this

`array = new DVD[6]`

- Is it a valid operation to insert `array[6]`? What about `array[10]`

- To find the length do:

```java
int capacity = array.length
```

### Basic Arrray Operations

- Now we have an understanding on what it is, we might want to perform using this software:

- **Insert:** A new DVD into the collection at a specific point
- **Delete:** delete it
- **Search:** look for one