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
            String output = "";
            if (input.contains("-")) {
                String[] parts = input.split("-");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                if (a >= 1 && a <= 10 && b >= 1 && b <= 10) {
                    result = a - b;
                    output = "" + result;
                }
            } else if (input.contains("+")) {
                String[] parts = input.split("+");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                if (a >= 1 && a <= 10 && b >= 1 && b <= 10) {
                    result = a + b;
                    output = "" + result;
                }
            } else if (input.contains("*")) {
                String[] parts = input.split("*");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                if (a >= 1 && a <= 10 && b >= 1 && b <= 10) {
                    result = a * b;
                    output = "" + result;
                }
            } else if (input.contains("/")) {
                String[] parts = input.split("/");
                int a = Integer.parseInt(parts[0]);
                int b = Integer.parseInt(parts[1]);
                if (a >= 1 && a <= 10 && b >= 1 && b <= 10) {
                    result = a / b;
                    output = "" + result;
                }
            } else {
                output = "throws Exception";
            }
            System.out.println(output);
            return output;
    }
}
