<p>We use the integers a, b, and n to create the following series:</p>
<p>(a+2°. b), (a +2° 6+2¹ b),..., (a+2º b+2²b+ ... + 2-1. b)</p>
<p>You are given q queries in the form of a, b, and n. For each query, print the series corresponding to the given a, b, and n values as a single line of n space-separated integers</p>
<h5>Input Format</h5>
<p>The first line contains an integer, q. denoting the number of queries.</p>
<p>Each line i of the q subsequent lines contains three space-separated integers describing the respective a, b₁, anden, values for that query.</p>
<h5>Constraints</h5>
<ul>
  <li>0 <= q <= 500</li>
  <li>0 <= a, b <= 50</li>
  <li>1 <= n <= 15</li>
</ul>
<h5>Output Format</h5>
<p>For each query, print the corresponding series on a new line. Each series must be printed in order as a single line of n space-separated integers.</p>
<h5>Sample Input</h5>

```
2
0 2 10
5 3 5
```
<h5>Sample Output</h5>

```
2 6 14 30 62 126 254 510 1022 2046
8 14 26 50 98
```
<p>Java solution:</p>

```Java
int sum = a;
for (int j = 0; j < n; j++) {
    sum += (int) Math.pow(2, j) * b;
    System.out.print(sum + " ");
}
System.out.println();
```
