# lab-1_3-23-16
import javax.swing.JOptionPane;

public class GuessANumJoption{

public static void main(String args[]){
	String message;

String number = JOptionPane.showInputDialog("Enter a number: ");

int i = Integer.parseInt(number);
int computerNum = 1 + (int) ( Math.random() * 10 );

message = String.format("Your number is %d\nComputer number is : %d\n", i, computerNum);
JOptionPane.showMessageDialog(null, message);


if ( i < computerNum)
  JOptionPane.showMessageDialog(null, "Your number is smaller than the computers.");
if ( i > computerNum)
	JOptionPane.showMessageDialog(null, "Your number is greater than the computers.");
if ( i == computerNum)
	JOptionPane.showMessageDialog(null, "Your number matches the computers.");
} }
