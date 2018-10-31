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
Successfully compiled /tmp/java_hNhMG0/exampleException.java <-- main method
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
Successfully compiled /tmp/java_hNhMG0/exampleException.java <-- main method
You can not divide by zero.
```
