# java-test-0002-final-15956-manasi
Final Project Assignment - This repository contains the complete final project code and documentation.
import java.util.Scanner;

public class HollowDiamondPattern {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the number of rows (odd number recommended): ");
        int rows = sc.nextInt();
        sc.close();

        //Ensure the number of rows is odd for a perfect diamond shape
        if (rows % 2 == 0) {
            rows++; 
        }

        int n = rows / 2 + 1; // Number of rows for the upper half

        // Upper half of the diamond
        for (int i = 1; i <= n; i++) {
            // Print leading spaces
            for (int j = 1; j <= n - i; j++) {
                System.out.print(" ");
            }

            // Print stars and inner spaces
            for (int k = 1; k <= 2 * i - 1; k++) {
                if (k == 1 || k == 2 * i - 1) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

        // Lower half of the diamond
        for (int i = n - 1; i >= 1; i--) {
            // Print leading spaces
            for (int j = 1; j <= n - i; j++) {
                System.out.print(" ");
            }

            // Print stars and inner spaces
            for (int k = 1; k <= 2 * i - 1; k++) {
                if (k == 1 || k == 2 * i - 1) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
  

           
