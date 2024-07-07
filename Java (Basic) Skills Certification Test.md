<p>Java solution:</p>

```Java
import java.util.Scanner;

abstract class Calculator {
    public abstract int add(int a, int b);
}
class Adder extends Calculator {
    public int add(int a, int b) {
        return a + b;
    }
}
```

```Java
import java.util.regex.Matcher;
import java.util.regex.Pattern;

public class Result {

    public static void typeCounter(String sentence) {
        int stringCount = 0;
        int integerCount = 0;
        int doubleCount = 0;

        String[] substrings = sentence.split("\\s+");

        Pattern stringPattern = Pattern.compile("^[a-zA-Z]+$");
        Pattern integerPattern = Pattern.compile("^\\d+$");
        Pattern doublePattern = Pattern.compile("^\\d+\\.\\d+$");

        for (String substring : substrings) {
            Matcher stringMatcher = stringPattern.matcher(substring);
            Matcher integerMatcher = integerPattern.matcher(substring);
            Matcher doubleMatcher = doublePattern.matcher(substring);

            if (stringMatcher.matches()) {
                stringCount++;
            } else if (integerMatcher.matches()) {
                integerCount++;
            } else if (doubleMatcher.matches()) {
                doubleCount++;
            }
        }

        System.out.println("string " + stringCount);
        System.out.println("integer " + integerCount);
        System.out.println("double " + doubleCount);
    }

    public static void main(String[] args) {
        String sentence = "give me 10 dollars";
        typeCounter(sentence);
    }
}
```

