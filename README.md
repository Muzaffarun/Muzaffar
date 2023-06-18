import java.util.Scanner;

public class PercentageCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите общую сумму: ");
        double total = scanner.nextDouble();

        System.out.print("Введите процент: ");
        double percent = scanner.nextDouble();

        double result = calculatePercentage(total, percent);
        System.out.println("Результат: " + result);
    }

    public static double calculatePercentage(double total, double percent) {
        return (percent / 100) * total;
    }
}
