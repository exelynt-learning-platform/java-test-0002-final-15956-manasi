# java-test-0002-final-15956-manasi
Final Project Assignment - This repository contains the complete final project code and documentation.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of rows: ");
        int n = sc.nextInt();

        // Upper half
        for (int i = 1; i <= n; i++) {

            // Spaces
            for (int j = i; j < n; j++) {
                System.out.print(" ");
            }

            // Increasing numbers
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }

            // Decreasing numbers
            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j);
            }

            System.out.println();
        }

        // Lower half
        for (int i = n - 1; i >= 1; i--) {

            // Spaces
            for (int j = n; j > i; j--) {
                System.out.print(" ");
            }

            // Increasing numbers
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }

            // Decreasing numbers
            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j);
            }

            System.out.println();
        }

        sc.close();
    }
}


           
