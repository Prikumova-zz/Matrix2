# Matrix2
import java.util.Scanner;
public class Matrix2 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println("Insert the number");
		Scanner in = new Scanner (System.in);
		int n = in.nextInt();
		int sum1 = 0;
		int sum2 = 0;
		int [] [] matrix = new int [n] [n];
		for (int i=0; i <n; i++) {
		
			for (int j = 0; j <matrix[i].length; j++) {
				
				matrix [i][j] = in.nextInt();
			}
		}
		for (int i = 0; i<matrix.length; i++) {
			sum1 += matrix [i][i];
			sum2 += matrix [i][n-1-i];
		}
				if (sum1 >=sum2) {
						System.out.println(sum1);
	}
				else {
						System.out.println(sum2);
		}
	}
	
}
