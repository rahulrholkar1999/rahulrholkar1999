- 👋 Hi, I’m @rahulrholkar1999
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
rahulrholkar1999/rahulrholkar1999 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

 Finding Prime number or Not
 
 package LogicalPro;
     
public class PrimeNum {

static void test(int n) {
		int count=0;
		for(int i=2; i<=n-1; i++) 
			{
				if(n%i==0)
				{
					count++;
				}
			}
			System.out.println(count);
			if(count==0)
			{
				System.out.println(+n+" is prime num");
			}
			else 
			{
				System.out.println(n+"is not prime num");
			}
			
		}
	public static void main(String[] args) {
	System.out.println("main started");
	test(2);

	}

}
// leap year

import java.util.*;

public class LeapYear {
	
	       
	
static  void test(int year){
		
	       {
		if(year%400==0 ||( year%4==0 && year%100!=0))
		{
			System.out.println(year+"-->is leap year");
		}
		else 
		{
			System.out.println(year+ " -->is not leap year");
		}
	       }
	       }
		
		public static void main(String[] args) {
			
			Scanner sc = new Scanner(System.in);
			System.out.println(" enter year");
			int year=sc.nextInt();
			//System.out.println(year);
			test(year);
	}

}
// SUM DIGITS
import java.util.*;

public class SumDigits {
	
	static void add(int num)
	{
		int sum=0;
		while(num>0)
		{
		int last= num%10;	
		sum=sum+last;
		num=num/10;
		
	}
		System.out.println("sum is ="+sum);
	}
	
	

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		System.out.println("enter num ");
		int num=sc.nextInt();
		
		
		add(num);
	}

}

// SPY NUMBER
import java.util.*;
public class SpyNumber {


	static void spy(int num)
	{
		
		{

			int temp=num;
			int sum=0;
			int prod=1;
			while(num>0)
			{
				int last=num%10;
				sum=sum+last;
				prod=prod*last;
				num=num/10;
			}



			if(sum==prod)
			{
				System.out.println(temp+" num is Spy number");
			}
			else
			{
				System.out.println(temp+" is not spy number");
			}
		}
	}




	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		System.out.println(" enter num");
		int num=sc.nextInt();
		spy(num);

	}
}

REVERSE STRING ---------



public class ReverseString {
	public static void main(String[] args) {
		String s="JAVA";
		char[] ch=s.toCharArray();
		for(int i=ch.length-1; i>=0; i--)
		{
			System.out.print(" "+ch[i]);
		}
		
	}

}








 

