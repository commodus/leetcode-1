<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../last-moment-before-all-ants-fall-out-of-a-plank "Last Moment Before All Ants Fall Out of a Plank")
　　　　　　　　　　　　　　　　
[Next >](../minimum-possible-integer-after-at-most-k-adjacent-swaps-on-digits "Minimum Possible Integer After at Most K Adjacent Swaps On Digits")

## [1504. Count Submatrices With All Ones (Medium)](https://leetcode.com/problems/count-submatrices-with-all-ones "统计全 1 子矩形")

<p>Given a&nbsp;<code>rows * columns</code>&nbsp;matrix <code>mat</code> of ones and zeros, return how many&nbsp;<strong>submatrices</strong> have all ones.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,0,1],
&nbsp;             [1,1,0],
&nbsp;             [1,1,0]]
<strong>Output:</strong> 13
<strong>Explanation:
</strong>There are <b>6</b> rectangles of side 1x1.
There are <b>2</b> rectangles of side 1x2.
There are <b>3</b> rectangles of side 2x1.
There is <b>1</b> rectangle of side 2x2. 
There is <b>1</b> rectangle of side 3x1.
Total number of rectangles = 6 + 2 + 3 + 1 + 1 = <strong>13.</strong>
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> mat = [[0,1,1,0],
&nbsp;             [0,1,1,1],
&nbsp;             [1,1,1,0]]
<strong>Output:</strong> 24
<strong>Explanation:</strong>
There are <b>8</b> rectangles of side 1x1.
There are <b>5</b> rectangles of side 1x2.
There are <b>2</b> rectangles of side 1x3. 
There are <b>4</b> rectangles of side 2x1.
There are <b>2</b> rectangles of side 2x2. 
There are <b>2</b> rectangles of side 3x1. 
There is <b>1</b> rectangle of side 3x2. 
Total number of rectangles = 8 + 5 + 2 + 4 + 2 + 2 + 1 = 24<strong>.</strong>
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,1,1,1,1,1]]
<strong>Output:</strong> 21
</pre>

<p><strong>Example 4:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,0,1],[0,1,0],[1,0,1]]
<strong>Output:</strong> 5
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= rows&nbsp;&lt;= 150</code></li>
	<li><code>1 &lt;= columns&nbsp;&lt;= 150</code></li>
	<li><code>0 &lt;= mat[i][j] &lt;= 1</code></li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Dynamic Programming](../../tag/dynamic-programming/README.md)]
  [[Stack](../../tag/stack/README.md)]
  [[Matrix](../../tag/matrix/README.md)]
  [[Monotonic Stack](../../tag/monotonic-stack/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
For each row i, create an array nums where:  if mat[i][j] == 0 then nums[j] = 0 else nums[j] = nums[j-1] +1.
</details>

<details>
<summary>Hint 2</summary>
In the row i, number of rectangles between column j and k(inclusive) and ends in row i, is equal to SUM(min(nums[j, .. idx])) where idx go from j to k.  Expected solution is O(n^3).
</details>
