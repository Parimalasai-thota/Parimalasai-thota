// PROGRAM TO PRINT SUM OF BOUNDAEIES IN 2D ARRAY
import java.util.Scanner;
public class Main
{
  public static void main (String[]args)
  {
	Scanner s = new Scanner (System.in);
	int row = s.nextInt ();
	int col = s.nextInt ();
	int arr[][] = new int[row][col];
	for (int i = 0; i < row; i++)
	  {
		for (int j = 0; j < col; j++)
		  {
			arr[i][j] = s.nextInt ();
		  }
	  }
	int sum_boundary = 0;
	for (int i = 0; i < row; i++)
	  {
		for (int j = 0; j < col; j++)
		  {
			if (i==0 || i==(row - 1) || j == 0 && (i >= 1 && i <= (row - 2)) || (j == row - 1 && (i >= 1 && i <= row - 2)))
			  {
				sum_zigzag += arr[i][j];
			  }

		  }
	  }
	System.out.println ("\nsum of Boundaries: "+ sum_boundary);
  }
}

