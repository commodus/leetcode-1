<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../design-skiplist "Design Skiplist")
　　　　　　　　　　　　　　　　
[Next >](../get-equal-substrings-within-budget "Get Equal Substrings Within Budget")

## [1207. Unique Number of Occurrences (Easy)](https://leetcode.com/problems/unique-number-of-occurrences "独一无二的出现次数")

<p>Given an array of integers <code>arr</code>, return <code>true</code> if the number of occurrences of each value in the array is <strong>unique</strong>, or <code>false</code> otherwise.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> arr = [1,2,2,1,1,3]
<strong>Output:</strong> true
<strong>Explanation:</strong>&nbsp;The value 1 has 3 occurrences, 2 has 2 and 3 has 1. No two values have the same number of occurrences.</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> arr = [1,2]
<strong>Output:</strong> false
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> arr = [-3,0,1,-3,1,1,1,-3,10,0]
<strong>Output:</strong> true
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= arr.length&nbsp;&lt;= 1000</code></li>
	<li><code>-1000 &lt;= arr[i] &lt;= 1000</code></li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Hash Table](../../tag/hash-table/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Find the number of occurrences of each element in the array using a hash map.
</details>

<details>
<summary>Hint 2</summary>
Iterate through the hash map and check if there is a repeated value.
</details>
