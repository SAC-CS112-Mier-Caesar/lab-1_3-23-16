# lab-6_3-23-16

import java.util.Scanner;
import javax.swing.JOptionPane;


public class Game { 
	public static void main(String[] args) { 
		Scanner input = new Scanner(System.in); 
		int userChoice; 
		int computerNum; 
		int playAgain;
		String computerPlay;
		String personPlay;
		String message;
		int count = 0;
		
		do {
		personPlay = JOptionPane.showInputDialog(null, "Welcome to a rock, paper, scissors game! \nPlease enter R, P, or S : ");
		computerNum = 1 + (int) (Math.random() * 3);
		
		if (computerNum == 1)
			computerPlay = "R";
		else
			computerPlay = (computerNum == 2) ? "P": "S";
		
		message = String.format("Computer play is: %s\n your choice is: %s\n ", computerPlay, personPlay);
		JOptionPane.showMessageDialog(null, message);
		
    
         if (personPlay.equalsIgnoreCase(computerPlay))
        	JOptionPane.showMessageDialog(null, "It's a tie!");
        else if ((personPlay.equalsIgnoreCase("r") && computerPlay.equalsIgnoreCase("p")) || (personPlay.equalsIgnoreCase("p") && computerPlay.equalsIgnoreCase("s")) || (personPlay.equalsIgnoreCase("s") && computerPlay.equalsIgnoreCase("r")))
            JOptionPane.showMessageDialog(null, "You lose.!");
        else
        	JOptionPane.showMessageDialog(null, "You Win!");
         count++;
		} while(count < 3);

}
}
