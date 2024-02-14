# Lab 3 Report
This lab focuses on identifying bugs in a program through testing and researching commands. 
* Part 1
Here we look at failure-inducing and non-failure-inducing input for a buggy program. I chose to look at a function that reverses the elements in an array.\n
`reverseInPlace()`\n
1. Failure-inducing input: A JUnit test that fails when testing `reverseInPlace()`\n
`public void testReverseInPlace1() {`\n
`  int[] input1 = { 1,2,3,4 };`\n
`  ArrayExamples.reverseInPlace(input1);`\n
`  assertArrayEquals(new int[]{ 4,3,2,1 }, input1);`\n
`}`\n
