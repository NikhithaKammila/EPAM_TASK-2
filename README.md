# EPAM_TASK-2
calculator program using java
@nikhitha

import java.util.Scanner;

public class Calculator {

    public static void main(String[] args) {

    	double n1, n2;
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter first number:");

        n1 = scanner.nextDouble();
        System.out.print("Enter second number:");
        n2 = scanner.nextDouble();

        System.out.print("Enter an operator (+, -, *, /): ");
        char operator = scanner.next().charAt(0);

        scanner.close();
        double a;

        switch(operator)
        {
            case '+':
            	a = n1 + n2;
                break;

            case '-':
            	a = n1 - n2;
                break;

            case '*':
            	a = n1 * n2;
                break;

            case '/':
            	a = n1 / n2;
                break;

            
            default:
                System.out.printf("You have entered wrong operator");
                return;
        }

        System.out.println(n1+" "+operator+" "+n2+": "+a);
    }
}
