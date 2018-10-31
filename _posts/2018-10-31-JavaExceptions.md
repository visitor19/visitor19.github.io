---
title: "Java Exceptions"
date: 2018-10-03
tags: [code]
excerpt: "Notes on Java Exception handling"
mathjax: true
---

>
>Checked / Unchecked Exceptions


Normal Statements; Critical Statement
Unchecked:
Run time exceptions

| Checked       | Unchecked           |
| ------------- |:-------------------:|
| IOExeption    | Runtime Exception   |
| SQLException  | -e                  |


The integer r has been set initially to 7. In the examples below we can see when the value of r prints as 7 it means that the code in the try-catch did not execute and that r is still at it's initial value.

### Example: Divide by zero error with no handled exception.

Input:
```java
public class exampleException{
  public static void main(String[] args){
    int a = 1;
    int b = 0;
    int r = 7;
    r = a/b;
     System.out.println("This code executes outside of the try-catch and after the exception is encountered. The value of r is "+r);}}
```
Output:
```xml
Exception in thread "main" java.lang.ArithmeticException: / by zero
	at exampleException.main(exampleException.java:6)
```
Note that the code with the print statement "This code executes outside"... did not execute.

### Example: Divide by zero error with handled exception.
Input:
```java
  public class exampleException{
    public static void main(String[] args){
      int a = 1;
      int b = 0;
      int r = 7;
      try {
        r = a/b; }
      catch(Exception e){
        System.out.println(e);}
     System.out.println("This code executes outside of the try-catch and after the exception is encountered. The value of r is "+r);}}
```


Output:
```xml
java.lang.ArithmeticException: / by zero
This code executes outside of the try-catch and after the exception is encountered. The value of r is 7
```

### Example: Divide by zero error with handled exception. Upon catching the error this time printing friendly a message instead of the error.
Input:
```java
public class exampleException{
   public static void main(String[] args){
     int a = 1;
     int b = 0;
     int r = 7;
     try {
       r = a/b; }
     catch(Exception e){
       System.out.println("You can not divide a number by zero.");}
     System.out.println("This code executes outside of the try-catch and after the exception is encountered. The value of r is "+r);}}
```

Output:
```xml
You can not divide a number by zero.
This code executes outside of the try-catch and after the exception is encountered. The value of r is 7
```
