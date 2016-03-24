# lab-1_3-23-16

import javax.swing.JOptionPane;

public class lab1 { 
  
  public static void main(String args[]){

    String number = JOptionPane.showInputDialog("Enter a number: ");
    
    int i = Integer.parseInt(number);
    computerNum = 1 + (int) ( Math.random() * 10 );

    
    if ( i < computerNum)
      String message = String.format("Your number is smaller than the computers.");
    if ( i > computerNum)
      String message = String.format("Your number is greater than the computers.");
    if ( i == computerNum)
      String message = String.format("Your number matches the computers.");
    
    
}
}
