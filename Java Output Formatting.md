<p>Java's System.out.printf function can be used to print formatted output. The purpose of this exercise is to test your understanding of formatting output using printf.</p>
<p>To get you started, a portion of the solution is provided for you in the editor; you must format and print the input to complete the solution.</p>
<h5>Input Format</h5>
<p>Every line of input will contain a String followed by an integer.</p>
<p>Each String will have a maximum of 10 alphabetic characters, and each integer will be in the inclusive range from 0 to 999.</p>
<h5>Output Format</h5>
<p>In each line of output there should be two columns:</p>
<p>The first column contains the String and is left justified using exactly 15 characters.</p>
<p>The second column contains the integer, expressed in exactly 3 digits; if the original input has less than three digits, you must pad your output's leading digits with zeroes.</p>
<h5>Sample Input</h5>

```
java 100
cpp 65
python 50
```
<h5>Sample Output</h5>

```
================================
java           100 
cpp            065 
python         050 
================================
```
<p>Java solution:</p>

```Java
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("================================");
        for (int i = 0; i < 3; i++) {
            String s1 = sc.next();
            int x = sc.nextInt();
            // Use printf to format the output
            System.out.printf("%-15s%03d%n", s1, x);
        }
        System.out.println("================================");
    }
}
```
