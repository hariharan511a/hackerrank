<p>Most HackerRank challenges require you to read input from stdin (standard input) and write output to stdout (standard output).</p>
<P>One popular way to read input from stdin is by using the Scanner class and specifying the Input Stream as System.in. For example:</P>

```Java
Scanner scanner = new Scanner(System.in);
String myString = scanner.next();
int myInt = scanner.nextInt();
scanner.close();

System.out.println("myString is: " + myString);
System.out.println("myInt is: " + myInt);
```
<p>The code above creates a Scanner object named scanner and uses it to read a String and an int. It then closes the Scanner object because there is no more input to read, and prints to stdout using System.out.println(String). So, if our input is: </p>

```Java
Hi 5
```
<p>Our code will print:</p>

```Java
myString is: Hi
myInt is: 5
```
<p>Alternatively, you can use the BufferedReader class.</p>
<h5>Task</h5>
<p>In this challenge, you must read 3 integers from stdin and then print them to stdout. Each integer must be printed on a new line. To make the problem a little easier, a portion of the code is provided for you in the editor below.</p>
<h5>Input Format</h5>
<p>There are  lines of input, and each line 3 contains a single integer.</p>
<h5>Sample Input</h5>

```Java
42
100
125
```
<h5>Sample Output</h5>

```Java
42
100
125
```
<p>Java solution:</p>

```Java
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        // Complete this line
        int b = scan.nextInt();
        int c = scan.nextInt();

        System.out.println(a);
        // Complete this line
        System.out.println(b);
        System.out.println(c);
    }
}
```
