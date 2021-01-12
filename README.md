# my first programm
import java.util.Scanner;
public class programm {
	public static void main (String[] args) {
		Scanner in = new Scanner(System.in);
		System.out.print("input size of array:");
		int size=in.nextInt();
		int[] myArray = new int[size];
		for (int i=0; i<myArray.length; i++) {
			int n=i+1;
			System.out.print("input number №" + n + " :" );
			myArray[i]=in.nextInt();
		}
		int min = 0;
		int max = 0;
		for (int i=0; i<myArray.length; i++) {
			if (max < myArray[i]) {
				max = myArray[i];
			}
		}
		min=max;
	    for (int i=0; i<myArray.length; i++) {	
		    if (min>myArray[i]) {
				min=myArray[i];
			}
		}
		System.out.println("maximum in array: "+max);
		System.out.println("minimum in array: "+min);	
	}

}
