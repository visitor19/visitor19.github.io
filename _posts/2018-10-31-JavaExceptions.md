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

```java
public class exampleException{
  public static void main(String[] args){
    int a = 1;
    int b = 0;
    int r = 0;
    r = a/b;
    System.out.println(r);}}
```
Output:
```xml
Exception in thread "main" java.lang.ArithmeticException: / by zero
	at exampleException.main(exampleException.java:6)
```


Input:
```java
  public class exampleException{
    public static void main(String[] args){
      int a = 1;
      int b = 0;
      int r = 0;
      try {
        r = a/b; }
      catch(Exception e){
        System.out.println(e);}
      System.out.println(r);}}
```


Output:
```xml
java.lang.ArithmeticException: / by zero
```

Input:
```java
  public class exampleException{
    public static void main(String[] args){
      int a = 1;
      int b = 0;
      int r = 0;
      try {
        r = a/b; }
      catch(Exception e){
        System.out.println("You can not divide by zero.");}
      System.out.println(r);}}
```


Output:
```xml
You can not divide by zero.
```
