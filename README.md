Printing Basic Incrementing Diamond Pattern (Inverted Sandwich)
In this program we’re going to code pyramid star pattern program .

The logic of this program is this take any number input from user and store it in variable n and then run the for loop start from 0 to i

start from j=n-i to j– and again take another for loop start from j=0 to j++ to print stars and after this take line changement statement after the end of main for loop

Java Program for Basic incrementing Diamond Pattern(Inverted Sandwich)
Algorithm:
Take the number of rows as input from the user and store it in any variable.(‘no‘ in this case). and take int count = no-2;
Run a loop ‘no’ number of times to iterate through each of the rows. From i=1 to i<=no. The loop should be structured as for (int i = 1; i <= no; i++) after this take another loop j for (int j = 1; j <= i; j++)  and take System.out.print(count); and take count++; take this to change line System.out.println(); 
Take another loop i for (int i = no; i>=1 ; i–) inside this take count– and take another for loop to print count variable for (int j = 1; j <=i; j++) and after this main for loop System.out.println();
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter no");
		int no = sc.nextInt();
        int count = no-2;
        
        for (int i = 1; i <= no; i++) {
			for (int j = 1; j <= i; j++) 
				System.out.print(count);
			count++;
			System.out.println();
		}
        for (int i = no; i>=1 ; i--) {
        	count--;
			for (int j = 1; j <=i; j++) 
				System.out.print(count);
			System.out.println();
		}

	}

}
