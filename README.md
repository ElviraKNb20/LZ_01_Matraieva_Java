# LZ_01_Matraieva_Java
import java.util.Scanner;
public class Main {
    public static void main(String[] args)
    {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введiть кiлькiсть чисел (n): ");
        int n=scanner.nextInt();
        if (n <= 0)
        {
            System.out.println("Кiлькiсть чисел повинна бути бiльше нуля.");
            return;
        }
        int min = Integer.MAX_VALUE;
        int max = Integer.MIN_VALUE;
        for (int i = 0; i < n; i++)
        {
            System.out.print("Введiть числo #" + (i+1) + ": ");
            int number = scanner.nextInt();
            if (number < min){
                min = number;
            }
            if (number > max){
                max = number;
            }
        }
        System.out.println("Найменше число: " + min);
        System.out.println("Найбільше число: " + max);
        scanner.close();
    }
}
