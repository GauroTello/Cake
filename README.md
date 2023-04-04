# Cake
Cake answer
import java.util.Scanner;

public class CakeMakingApp {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("Welcome to the Cake Making App!");

        // Get user input for the type of cake they want to make
        System.out.println("What type of cake would you like to make?");
        String cakeType = input.nextLine();

        // Get user input for the number of eggs needed
        System.out.println("How many eggs are needed for the recipe?");
        int eggsNeeded = input.nextInt();

        // Get user input for the amount of flour needed
        System.out.println("How many cups of flour are needed for the recipe?");
        double flourNeeded = input.nextDouble();

        // Display the cake recipe to the user
        System.out.println("\nGreat! Here's the recipe for " + cakeType + ":");
        System.out.println(" - " + eggsNeeded + " eggs");
        System.out.println(" - " + flourNeeded + " cups of flour");

        // Calculate the cost of ingredients
        double eggCost = 0.10;  // cost per egg in dollars
        double flourCost = 0.25;  // cost per cup of flour in dollars
        double totalCost = eggsNeeded * eggCost + flourNeeded * flourCost;

        // Display the total cost to the user
        System.out.printf("\nThe total cost of ingredients for %s is $%.2f", cakeType, totalCost);
    }
}
