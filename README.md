# Exam-Problem-1

Problem-1:  Create a small calculator which performs operations such as Addition, Subtraction, Multiplication and Division using class.
    Calculator inputs :> ‘a’, ‘b’ and ‘type of operation’
    Datatype :> ‘a’ = double, ‘b’ = double, ‘type of operation’ = string

import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    char operator;
    Double number1, number2, result;

    // create an object of Scanner class
    Scanner input = new Scanner(System.in);

    // ask users to enter operator
    System.out.println("Choose an operator: +, -, *, or /");
    operator = input.next().charAt(0);

    // ask users to enter numbers
    System.out.println("Enter the first number");
    number1 = input.nextDouble();

    System.out.println("Enter the second number");
    number2 = input.nextDouble();

    switch (operator) {

      // Addition between numbers
      case '+':
        result = number1 + number2;
        System.out.println(number1 + " + " + number2 + " = " + result);
        break;

      // Subtraction between numbers
      case '-':
        result = number1 - number2;
        System.out.println(number1 + " - " + number2 + " = " + result);
        break;

      // Multiplication between numbers
      case '*':
        result = number1 * number2;
        System.out.println(number1 + " * " + number2 + " = " + result);
        break;

      // Division between numbers
      case '/':
        result = number1 / number2;
        System.out.println(number1 + " / " + number2 + " = " + result);
        break;

      default:
        System.out.println("Invalid operator!");
        break;
    }

    input.close();
  }
}

Output 1
Choose an operator: +, -, *, or /
*
Enter the first number
3
Enter the second number
9
3.0 * 9.0 = 27.

Output 2
Choose an operator: +, -, *, or /
+
Enter the first number
21
Enter the second number
8
21.0 + 8.0 = 29.0

Output 3
Choose an operator: +, -, *, or /
-
Enter the first number
9
Enter the second number
3
9.0 - 3.0 = 6.0

Output 4
Choose an operator: +, -, *, or /
/
Enter the first number
24
Enter the second number
8
24.0 / 8.0 = 3.0


