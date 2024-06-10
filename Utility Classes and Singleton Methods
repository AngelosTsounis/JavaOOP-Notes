1. Instance control classes / Utility classes / Static Factory classes


Instance Control

The number of instances a class contains determines their type as well. For example is a class has 0 instanses it's called a utility class.
Utility classes contain:
1. Only public methods and no data while they are non-instantiable.
2. They are non-instantiable so we use a private constructor.
3. They only contain public static methods. For example this MathHelper class:

public class MathHelper {
 
    private MathHelper() {
    
    }
    public static int findMax(int[] numbers) {
        int max = numbers[0];

        for(int number : numbers) {
            if (number > max) {
                max = number;
            }
        }
        return max;
    }

    public static int findMin(int[] numbers) {
        int min = numbers[0];

        for(int number : numbers) {
            if (number < min) {
                min = number;
            }
        }
        return min;
    } 
} 

If a class contains only one istance it's called Singleton and we create the instance within the class. It has a private default constructor and public methods: 

public class Logger {
  private static final Logger INSTANCE = new Logger();

  private Logger() {}

    public static Logger getInstance() {
      return INSTANCE;
    }

    public void logMessage() {
        System.out.println("This is the Logger message");
    }
}

We also have the static factory methods. They contain a public default constructor and all the methods are static. If a method is static it can be used whithin the whole package.

public class ValidationUtils {

    private ValidationUtils() {

    }
    public static boolean validateNum(int num) {
        boolean check = false;
        if(num > 1 && num < 10) {
            return check = true;
        }
       return check;
    }

    public static boolean isStringLengthValid(String input) {
        if (input == null) {
            return false;
        }
        int length = input.length();
        return length >= 1 && length <= 31;
    }
}
