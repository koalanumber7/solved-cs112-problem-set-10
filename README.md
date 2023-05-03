Download Link: https://assignmentchef.com/product/solved-cs112-problem-set-10
<br>
<strong>Problem Set 10</strong>

<strong>Heap</strong>

<ol>

 <li>Given the following sequence of integers:</li>

</ol>

12, 19, 10, 4, 23, 7, 45, 8, 15

<ol>

 <li>Build a heap by inserting the above set, one integer at a time, in the given sequence. Show the heap after every insertion. How many comparisons in all did it take to build the heap?</li>

 <li>Perform successive <em>delete</em> operations on the heap constructed in the previous step, until the heap is empty. Show the heap after every deletion. How many comparisons in all did it take to perform these deletions?</li>

</ol>

<ol start="2">

 <li>Suppose we have a (<strong>max</strong>) heap that stores integers. (By contrast, in a “min” heap the key at any node is <em>less than or equal to</em> the key at its children, so the <em>smallest</em> valued key is at the top of the heap.) Then, given an integer <em>k</em>, we would like to print all the values in this heap that are <em>greater than k</em>. Implement the following method to do this.</li>

</ol>




public void printGreater(int[] H, int n, int k) {

/* your code here */     }

<em>H</em> is the array storage for the max heap, and <em>n</em> is the number of entries in the heap.

<em>Note: The challenge is to do this efficiently. Use the heap order to reduce the number of entries of the heap to be examined.</em>

<ol start="3">

 <li>Consider a max heap that only supports the operations <strong>insert</strong>, <strong>deleteMax</strong>, <strong>size</strong>, and <strong>isEmpty</strong>. A client of the heap wants to update the priority of an entry in the heap. Since there is no search operation, the only way to accomplish the update is this:</li>

</ol>

Perform successive <strong>deleteMax</strong> operations until the entry is extracted Update the entry’s priority

<strong>Insert</strong> the entry, as well as all the other deleted entries back into the heap

What would be the worst case running time (big <em>O</em>) of this update process on a heap with <em>n</em> entries?

<ol start="4">

 <li>Suppose you are given two heaps, stored in arrays. Write a method to merge them into a single heap, and return this heap. The original heaps are not modified:</li>

</ol>

public static &lt;T extends Comparable&lt;T&gt;&gt; T[] merge(T[] heap1, T[] heap2) {

// COMPLETE THIS METHOD

}