package testprgm;
import java.util.Arrays;
import java.util.Scanner;

public class FindMissingNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input array from the user
        System.out.print("Enter the array elements separated by spaces: ");
        String input = scanner.nextLine();
        String[] strArray = input.split(" ");
        int[] array = new int[strArray.length];

        for (int i = 0; i < strArray.length; i++) {
            array[i] = Integer.parseInt(strArray[i]);
        }

        // Sort the array
        Arrays.sort(array);

        // Find and print the consecutive missing number
        int missingNumber = findMissingNumber(array);
        System.out.println("The consecutive missing number is: " + missingNumber);
    }

    // Function to find the consecutive missing number
    private static int findMissingNumber(int[] array) {
        int n = array.length;
        for (int i = 0; i < n - 1; i++) {
            if (array[i + 1] - array[i] != 1) {
                return array[i] + 1;
            }
        }
        // If no missing number is found, return -1 or handle as needed
        return -1;
    }
}


