<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../stone-game-vii "Stone Game VII")
　　　　　　　　　　　　　　　　
[Next >](../count-ways-to-distribute-candies "Count Ways to Distribute Candies")

## [1691. Maximum Height by Stacking Cuboids  (Hard)](https://leetcode.com/problems/maximum-height-by-stacking-cuboids "堆叠长方体的最大高度")

<p>Given <code>n</code> <code>cuboids</code> where the dimensions of the <code>i<sup>th</sup></code> cuboid is <code>cuboids[i] = [width<sub>i</sub>, length<sub>i</sub>, height<sub>i</sub>]</code> (<strong>0-indexed</strong>). Choose a <strong>subset</strong> of <code>cuboids</code> and place them on each other.</p>

<p>You can place cuboid <code>i</code> on cuboid <code>j</code> if <code>width<sub>i</sub> &lt;= width<sub>j</sub></code> and <code>length<sub>i</sub> &lt;= length<sub>j</sub></code> and <code>height<sub>i</sub> &lt;= height<sub>j</sub></code>. You can rearrange any cuboid&#39;s dimensions by rotating it to put it on another cuboid.</p>

<p>Return <em>the <strong>maximum height</strong> of the stacked</em> <code>cuboids</code>.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<p><strong><img alt="" src="https://assets.leetcode.com/uploads/2019/10/21/image.jpg" style="width: 420px; height: 299px;" /></strong></p>

<pre>
<strong>Input:</strong> cuboids = [[50,45,20],[95,37,53],[45,23,12]]
<strong>Output:</strong> 190
<strong>Explanation:</strong>
Cuboid 1 is placed on the bottom with the 53x37 side facing down with height 95.
Cuboid 0 is placed next with the 45x20 side facing down with height 50.
Cuboid 2 is placed next with the 23x12 side facing down with height 45.
The total height is 95 + 50 + 45 = 190.
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> cuboids = [[38,25,45],[76,35,3]]
<strong>Output:</strong> 76
<strong>Explanation:</strong>
You can&#39;t place any of the cuboids on the other.
We choose cuboid 1 and rotate it so that the 35x3 side is facing down and its height is 76.
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> cuboids = [[7,11,17],[7,17,11],[11,7,17],[11,17,7],[17,7,11],[17,11,7]]
<strong>Output:</strong> 102
<strong>Explanation:</strong>
After rearranging the cuboids, you can see that all cuboids have the same dimension.
You can place the 11x7 side down on all cuboids so their heights are 17.
The maximum height of stacked cuboids is 6 * 17 = 102.
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>n == cuboids.length</code></li>
	<li><code>1 &lt;= n &lt;= 100</code></li>
	<li><code>1 &lt;= width<sub>i</sub>, length<sub>i</sub>, height<sub>i</sub> &lt;= 100</code></li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Dynamic Programming](../../tag/dynamic-programming/README.md)]
  [[Sorting](../../tag/sorting/README.md)]

### Similar Questions
  1. [The Number of Weak Characters in the Game](../the-number-of-weak-characters-in-the-game) (Medium)

### Hints
<details>
<summary>Hint 1</summary>
Does the dynamic programming sound like the right algorithm after sorting?
</details>

<details>
<summary>Hint 2</summary>
Let's say box1 can be placed on top of box2. No matter what orientation box2 is in, we can rotate box1 so that it can be placed on top. Why don't we orient everything such that height is the biggest?
</details>
