<h5>Output Format</h5>
<p>There are three lines of output:</p>
<ol>
  <li>On the first line, print String: followed by the unaltered String read from stdin.</li>
  <li>On the second line, print Double: followed by the unaltered double read from stdin.</li>
  <li>On the third line, print Int: followed by the unaltered integer read from stdin.</li>
</ol>
<p>To make the problem easier, a portion of the code is already provided in the editor.</p>
<p>Note: If you use the nextLine() method immediately following the nextInt() method, recall that nextInt() reads integer tokens; because of this, the last newline character for that line of integer input is still queued in the input buffer and the next nextLine() will be reading the remainder of the integer line (which is empty).</p>
<h5>Sample Input</h5>

```
42
3.1415
Welcome to HackerRank's Java tutorials!
```
<h5>Sample Output</h5>

```Java
String: Welcome to HackerRank's Java tutorials!
Double: 3.1415
Int: 42
```
<p>Java solution:</p>

```Java
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int i = scan.nextInt();

        // Write your code here.
        float d = scan.nextFloat();
        scan.nextLine();
        String s = scan.nextLine();
        
        System.out.println("String: " + s);
        System.out.println("Double: " + d);
        System.out.println("Int: " + i);
    }
}
```
