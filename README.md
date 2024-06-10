# JavaOOP-Notes

1. Instance control classes / Utility classes / Static Factory classes


Instance Control

The number of instances a class contains determines their type as well. For example is a class has 0 instanses it's called a utility class.
Utility classes contain:
1. Only public methods and no data while they are non-instantiable.
2. They are non-instantiable so we use a private constructor.
3. They only contain public static methods. For example this MathHelper class:
4. public class MathHelper {

public class MathHelper {


    private MathHelper() {}
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

    public static int averageNum(int[] numbers) {
        int sum = 0;

        for(int number : numbers) {
             sum = sum + number;
        }
        return sum / numbers.length;
    }
}
