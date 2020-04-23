# Pemrograman-Berorientasi-Obyek1
Source Code JAVA Algebra: quadratic equations

import java.util.Scanner;
public class Algebra{

  public static void main(String[] Strings) {

        Scanner input = new Scanner(System.in);

            System.out.print("Input a, b, c: ");
            double a = input.nextDouble();
            double b = input.nextDouble();
            double c = input.nextDouble();
            double result = b * b - 4.0 * a * c;

            if (result > 0.0) {
                double r1 = (-b + Math.pow(result, 0.5)) / (2.0 * a);
                double r2 = (-b - Math.pow(result, 0.5)) / (2.0 * a);
                System.out.println("The roots are " + r1 + " and " + r2);
            } else if (result == 0.0) {
                double r1 = -b / (2.0 * a);
                System.out.println("The root is " + r1);
            } else {
                System.out.println("The equation has no real roots.");
            }
    }
}

