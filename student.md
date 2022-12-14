package com.tcc.java.programs;
 
import java.util.Scanner;
 
/**
 * Java Program to find average and percentage marks of N subjects
 */
public class AverageMarks {
    public static void main(String[] args) {
        int count, i;
        float totalMarks = 0, percentage, average;
        Scanner scanner;
        scanner = new Scanner(System.in);
 
        System.out.println("Enter number of Subject");
        count = scanner.nextInt();
 
        System.out.println("Enter Marks of " + count + " Subject");
        for (i = 0; i < count; i++) {
            totalMarks += scanner.nextInt();
        }
 
        average = totalMarks / count;
        // Each subject is of 100 Marks
        percentage = (totalMarks / (count * 100)) * 100;
 
        System.out.println("Total Marks : " + totalMarks);
        System.out.println("Average Marks : " + average);
        System.out.println("Percentage : " + percentage);
    }
}
