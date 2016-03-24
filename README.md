import java.util.Arrays;
import java.util.Scanner;
import javax.swing.JOptionPane;


public class Game { 
	public static void main(String[] args) { 
		int[] array;
		int average;
		array = new int[6];
		
		array[0] = 123;
		array[1] = 456;
		array[2] = 479;
		array[3] = 135;
		array[4] = 246;
		array[5] = 135;
		
		Arrays.sort(array);
		average = (array[0] + array[1] + array[2] + array[3] + array[4] + array[5])/6;
		for (int i = 0; i < array.length; i++){
			System.out.println("Num: " + array[i]);
			
		}
		System.out.printf("The average is: %d ", average);

}
}
