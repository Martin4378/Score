# Score

import java.util.Scanner;

public class P22_Score {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int number = Integer.parseInt(scanner.nextLine());

        double bonus = 0;

        if (number <= 100) {
            bonus = bonus + 5;
        }
        else if (number <= 1000) {
            bonus = number * 20 / 100.0;
        } else if( number > 1000) {
            bonus = number * 10 / 100.0;
        }

        if (number % 2 == 0) {
            bonus = bonus + 1;

        } else {
            if (number % 10 == 5) {
                bonus += 2;
            }


        }
        System.out.println(bonus);
        System.out.println(bonus + number);
    }

}

