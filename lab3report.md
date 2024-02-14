# Lab 3 Report

This lab focuses on identifying bugs in a program through testing and researching commands. 

* Part 1

Here we look at failure-inducing and non-failure-inducing input for a buggy program. I chose to look at a function that reverses the elements in an array.  
`reverseInPlace()`  

1. Failure-inducing input: A JUnit test that fails when testing `reverseInPlace()`
Using the input array `{ 1,2,3,4 }`, the function will produce `{ 4,3,3,4 }` rather than the correct reversed array `{ 4,3,2,1 }`.

```
public void testReverseInPlaceFail() {  
    int[] input1 = { 1,2,3,4 };  
    ArrayExamples.reverseInPlace(input1);  
    assertArrayEquals(new int[]{ 4,3,2,1 }, input1);  
}
```

2. Non-failure-inducing input: A JUnit test that succeeds when testing `reverseInPlace()`
Using the input array `{ 3 }`, the function will produce `{ 3 }`, which is the correct reversed array.

```
public void testReverseInPlaceSuccess() {  
    int[] input1 = { 3 };  
    ArrayExamples.reverseInPlace(input1);  
    assertArrayEquals(new int[]{ 3 }, input1);  
}
```
3. Symptom of the code: We observe that one of the tests fail (`testReverseInPlaceFail()`) and one of them passes (`testReverseInPlaceSuccess()`).
![Image](JUnit-test-output.png) 

