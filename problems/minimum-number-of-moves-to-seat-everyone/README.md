<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../maximum-alternating-subarray-sum "Maximum Alternating Subarray Sum")
　　　　　　　　　　　　　　　　
[Next >](../remove-colored-pieces-if-both-neighbors-are-the-same-color "Remove Colored Pieces if Both Neighbors are the Same Color")

## [2037. Minimum Number of Moves to Seat Everyone (Easy)](https://leetcode.com/problems/minimum-number-of-moves-to-seat-everyone "使每位学生都有座位的最少移动次数")

<p>There are <code>n</code> seats and <code>n</code> students in a room. You are given an array <code>seats</code> of length <code>n</code>, where <code>seats[i]</code> is the position of the <code>i<sup>th</sup></code> seat. You are also given the array <code>students</code> of length <code>n</code>, where <code>students[j]</code> is the position of the <code>j<sup>th</sup></code> student.</p>

<p>You may perform the following move any number of times:</p>

<ul>
	<li>Increase or decrease the position of the <code>i<sup>th</sup></code> student by <code>1</code> (i.e., moving the <code>i<sup>th</sup></code> student from position&nbsp;<code>x</code>&nbsp;to <code>x + 1</code> or <code>x - 1</code>)</li>
</ul>

<p>Return <em>the <strong>minimum number of moves</strong> required to move each student to a seat</em><em> such that no two students are in the same seat.</em></p>

<p>Note that there may be multiple seats or students in the <strong>same </strong>position at the beginning.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> seats = [3,1,5], students = [2,7,4]
<strong>Output:</strong> 4
<strong>Explanation:</strong>&nbsp;The students are moved as follows:
- The first student is moved from from position 2 to position 1 using 1 move.
- The second student is moved from from position 7 to position 5 using 2 moves.
- The third student is moved from from position 4 to position 3 using 1 move.
In total, 1 + 2 + 1 = 4 moves were used.
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> seats = [4,1,5,9], students = [1,3,2,6]
<strong>Output:</strong> 7
<strong>Explanation:</strong>&nbsp;The students are moved as follows:
- The first student is not moved.
- The second student is moved from from position 3 to position 4 using 1 move.
- The third student is moved from from position 2 to position 5 using 3 moves.
- The fourth student is moved from from position 6 to position 9 using 3 moves.
In total, 0 + 1 + 3 + 3 = 7 moves were used.
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> seats = [2,2,6,6], students = [1,3,2,6]
<strong>Output:</strong> 4
<strong>Explanation:</strong>&nbsp;The students are moved as follows:
- The first student is moved from from position 1 to position 2 using 1 move.
- The second student is moved from from position 3 to position 6 using 3 moves.
- The third student is not moved.
- The fourth student is not moved.
In total, 1 + 3 + 0 + 0 = 4 moves were used.
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>n == seats.length == students.length</code></li>
	<li><code>1 &lt;= n &lt;= 100</code></li>
	<li><code>1 &lt;= seats[i], students[j] &lt;= 100</code></li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Sorting](../../tag/sorting/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Can we sort the arrays to help solve the problem?
</details>

<details>
<summary>Hint 2</summary>
Can we greedily match each student to a seat?
</details>

<details>
<summary>Hint 3</summary>
The smallest positioned student will go to the smallest positioned chair, and then the next smallest positioned student will go to the next smallest positioned chair, and so on.
</details>
