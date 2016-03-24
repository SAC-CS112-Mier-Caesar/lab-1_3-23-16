# lab-1_3-23-16
import java.util.Scanner;

public class Game { 
	public static void main(String[] args) { 
		Scanner input = new Scanner(System.in); 
		int userChoice; 
		int computerNum; 
		int playAgain; 
		computerNum = 1 + (int) (Math.random() * 3);

    System.out.println("Lets play Rock, Paper, Scissors! Ready?..");
    do {
        System.out.print("Rock, Paper, or Scissors?(1=Rock, 2=Paper, 3=Scissors): ");

        userChoice = input.nextInt();

        if (userChoice == computerNum)
        	System.out.println("It's a tie!");
        else if ((computerNum == 1 && userChoice == 3) || (computerNum == 2 && userChoice == 1) || (computerNum == 3 && userChoice == 2) )
            System.out.println("You lose.!");
        else
        	System.out.println("You Win!");

        System.out.print("Want to play again? (1=Yes, 2=No): ");
        playAgain = input.nextInt();
    } while (playAgain == 1);
}
}
