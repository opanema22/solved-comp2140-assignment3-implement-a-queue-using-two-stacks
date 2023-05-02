Download Link: https://assignmentchef.com/product/solved-comp2140-assignment3-implement-a-queue-using-two-stacks
<br>
<strong>Code you can use: </strong>You are permitted to use and modify the code your instructor gave you in class the completed assignments and labs. Of course, you must use the code we provided to you below. You are NOT permitted to use code from any other source, You are NOT permitted to show or give your code to any other student. Any other code you need for this assignment, you must write for yourself. We encourage you to write ALL the code for this assignment yourself, based on your understanding of the algorithms — you will learn the material much better if you write the code yourself. <strong>Files: </strong>Familiarize yourself with the code in the following files.

<ol>

 <li>java: You are to edit this file to implement a queue using two stacks as described below. This is the first file to be submitted.</li>

 <li>java: This class implements a stack, with the usual operations push, pop, and isEmpty. You should not edit this file.</li>

 <li>java: This class implements a linked-list node. This code is similar to that used in Lab 2, Lab 3, and Assignment 2. You should not edit this file.</li>

 <li>java: This class implements an exception thrown when an attempt is made to perform a pop or dequeue operation on an empty stack or queue. This code is similar to that used in Lab 3. You should not edit this file.</li>

 <li>java: This code shows an example of how to instantiate and use the class MyQueue. You may edit this file to help you test your code. This is the second file to be submitted.</li>

</ol>

<strong>What you should implement:</strong>

<ol>

 <li>You are to edit the file MyQueue.java as described below. A queue can be implemented using two stacks, stack1 and stack2. The enqueue operation pushes the new item onto stack1, while the dequeue operation pops the top item from stack2 and returns it. If stack2 becomes empty, the content of stack1 is moved to stack2 such that its order on stack2 is the reverse from what it was on stack1. Note that this is not an efficient implementation of a queue; you saw in lecture how to implement enqueue and dequeue with O(1) worst-case time. The goal of this assignment is for you to examine how to use the existing functionality of stacks to solve other problems, such as implementing a queue.

  <ul>

   <li>Add declarations for two instance variables stack1 and stack2 of type MyStack&lt;E&gt;. Both should be declared protected.</li>

   <li>Within the constructor, add two statements that initialize stack1 and stack2 by assigning them respective references to two new instances of the class MyStack&lt;E&gt;, each of which is a new empty stack.</li>

   <li>Add code to the method enqueue such that it pushes elem onto stack1.</li>

   <li>Add code to the method transferStacks to move the content of stack1 to stack2 such that its order on stack2 is the reverse from what it was on stack1. stack1 should be empty after a call to transferStacks.</li>

   <li>Add code to the method dequeue to a) check whether stack2 is empty and, if so, to call transferStacks, and b) to pop the top item from stack2 and store it in result.</li>

   <li>Add code to the method isEmpty such that it sets the value of result to true if and only if the queue is empty. Your code should only call accessor methods on the stacks.</li>

  </ul></li>

</ol>

Figure 1: Java collection hierarchy. See <a href="https://docs.oracle.com/javase/tutorial/collections/interfaces/index.html">https://docs.oracle.com/javase/tutorial/collections/interfaces/index.html.</a>

Note that Map is omitted in this image (ask yourself, why?). Image from dzone.com

<ol start="2">

 <li>You are to edit the A3&lt;your last name&gt;&lt;your first name&gt;.java. Please write your code in the main function where indicated. Most of these questions are to show you the utility of existing collections (Figure 1).

  <ul>

   <li>Manually search the ArrayList class (you can find the implementation by going to the source code, or searching and reading the class file online) to find the function that can be used to get the element at a given index.</li>

   <li>Search the ArrayList class to find a way (more than 1 way exist) to add all books in store1 to store2 with a single line of code.</li>

   <li>2c, 2d and 2e below do not require any coding.</li>

   <li>In your report at the end of the assignment, write one sentence about the difference between linkedlist and arraylist.</li>

   <li>In your report at the end of the assignment, write one sentence about the difference between store3 and store4. What are the methods that can be called on store4, but not on store3?</li>

   <li>In your report at the end of the assignment, write two sentences about the difference between store3 and store4. What is the advantage of using the LinkedList declaration in store4? in turn, what is the disadvantage?</li>

  </ul></li>

</ol>

<strong>Concerns.</strong>

Please avoid magical numbers in your code. There should be only ONE return per method. See the programming standards (under content/course documents) file on UMLearn, and follow the suggestions. Assignments will be graded by considering these standards. Your code must not give any warnings or errors when compiled and run.