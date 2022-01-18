# sort_numbers
import java.util.Scanner;

/*lili*/


public class sortnumbers {

	public static void main(String[] args) {
		 Scanner keyboard= new Scanner(System.in);
		 System.out.println("please input numbers and I will sort them");
		int number=keyboard.nextInt();
		int[] arr=new int[number];
		 for(int i=0;i<number; i++)
		 {
			 System.out.println("value"+i);
			 arr[i]=keyboard.nextInt();
		 }
		 
		 boolean isSorted=true;
		 while(isSorted) 
		 {
			 isSorted=false;
			 for(int i=0;i<number-1; i++)
			 {
			 if(arr[i]<arr[i+1])
			 {
				 int temp =arr[i];
				 arr[i]=arr[i+1];
				 arr[i+1]=temp;
				 isSorted=true;
				 
			 }
			 }
			 
		 }
		 
		 for(int i=0;i<number; i++)
		 {
			 System.out.println(arr[i]);
		 }
			 

	}

}
