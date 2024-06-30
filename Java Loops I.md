<h5>Objective</h5>
<p>In this challenge, we're going to use loops to help us do some simple math.</p>
<h5>Task</h5>
<p>Given an integer, N, print its first 10 multiples. Each multiple N x i (where 1 ≤ i ≤ 10) should be printed on a new line in the form: N x i = result.</p>
<h5>Input Format</h5>
<p>A single integer, N.</p>
<h5>Constraints</h5>
<ul>
  <li>2 ≤ N ≤ 20</li>
</ul>
<h5>Output Format</h5>
<p>Print 10 lines of output; each line i (where 1 <= i <= 10 ) contains the result of N x i in the form:</p>
<p>N x i = result.</p>
<h5>Sample Input</h5>
<p>2</p>
<h5>Sample Output</h5>

```
2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
```
<p>Java solution:</p>

```Java
for (int i = 1; i <= 10; i++) {
    System.out.println(N + " x " + i + " = " + (N * i));
}
```
