# Calcul
test
import java.util.Scanner;

public class Main {
    public static String calc(String input) {
            Scanner scanner;
            scanner = new Scanner(System.in);
            input = scanner.nextLine();
            input = input.replaceAll(" ", "");
            int result;
            String output;
            if (input.contains("-")) {
                String[] parts = input.split("-");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                result = a - b;
                output = "" + result;
            } else if (input.contains("+")) {
                String[] parts = input.split("+");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                result = a + b;
                output = "" + result;
            } else if (input.contains("*")) {
                String[] parts = input.split("*");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                result = a * b;
                output = "" + result;
            } else if (input.contains("/")) {
                String[] parts = input.split("/");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                result = a / b;
                output = "" + result;
            } else {
                output = "throws Exception";
            }
            System.out.println(output);
            return output;
        }
    }
