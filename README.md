# Sum-of-even-and-odd-coding_ninjas-java
import java.util.* ;
import java.io.*; 

public class Solution {

	public static int[] sumOfEvenOdd(long num, int evenSum, int oddSum) {

		int[] a = new int[2];   
		int digit=0;        
		while(num>0){            
			digit=(int)num%10;                        
			if(digit%2!=0){
				oddSum = oddSum+digit;
			}                
		    	            
			else{
				evenSum=evenSum+digit;
			}
			num=num/10;			          
		}
		a[0] = evenSum;
		a[1] = oddSum;
		 return a;
		 
	}
}
