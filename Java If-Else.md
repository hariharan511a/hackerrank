<p>In this challenge, we test your knowledge of using if-else conditional statements to automate decision-making processes. An if-else statement has the following logical flow:</p>

![1446563087-4ec019a919-332px-If-Then-Else-diagram svg](https://github.com/hariharan511a/hackerrank/assets/171676691/652239ee-5c85-450e-ad00-bcc083d8f4d0)

<h5>Task</h5>
<p>Given an integer, n, perform the following conditional actions:</p>
<ul>
  <li>If n is odd, print Weird</li>
  <li>If n is even and in the inclusive range of 2 to 5, print Not Weird</li>
  <li>If n is even and in the inclusive range of 6 to 20, print  Weird</li>
  <li>If  is even and greater than , print Not Weird</li>
</ul>
<p>Complete the stub code provided in your editor to print whether or not n is weird.</p>
<h5>Input Format</h5>
<p>A single line containing a positive integer, n.</p>
<h5>Constraints</h5>
<ul>
  <li>1 ≤ n ≤ 100</li>
</ul>
<h5>Output Format</h5>
<p>Print Weird if the number is weird; otherwise, print Not Weird.</p>
<h5>Sample Input 0</h5>
<p>3</p>
<h5>Sample Input 0</h5>
<p>Weird</p>
<h5>Sample Input 1</h5>
<p>24</p>
<h5>Sample Input 1</h5>
<p>Not Weird</p>
<h5>Explanation</h5>
<p>Sample Case 0: n = 3</p>
<p>n is odd and odd numbers are weird, so we print Weird.</p>
<p>Sample Case 1: n = 24</p>
<p>n > 20 and n is even, so it isn't weird. Thus, we print Not Weird.</p>
<p>Java solution:</p>

```Java
if (n % 2 == 1) {
    System.out.println("Weird");
} else {
    if (n >= 6 && n <= 20) {
        System.out.println("Weird");
    } else {
        System.out.println("Not Weird");
    }
}
```

