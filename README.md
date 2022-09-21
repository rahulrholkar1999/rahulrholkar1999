_finding Prime number
 package LogicalPro;

public class PrimeNum {


	static  void test(int n) {

		for(int i=2; i<=n; i++) 
		{
			int count=0;
			for(int j=2; j<i; j++) {
				if(i%j==0)
				{
					count++;
				}
			}
			if(count==0)
			{
				System.out.println(i+" ");
			}
		}
	}

	public static void main(String[] args) {
		System.out.println("main started");
		test(20);

	}

}
_____________________________________________________________________________________________________________________

import java.util.Scanner;
public class AmstrongNum {

	static void test(int num)
	{
		int res=0;
		int temp=num;
		while(num>0)
		{
			int rem=num%10;
			res=res+(rem*rem*rem);
			num=num/10;
		}


		if(temp==res)
		{
			System.out.println(temp+" is Amstrong Numbers");
		}
		else
		{
			System.out.println(temp+" not Amstrong num");
		}


	}
	public static void main(String[] args) {
		Scanner sc =new Scanner(System.in);
		System.out.println("enter num");
		int num=sc.nextInt();
		test(num);

	}

}
_____________________________________________________________________________________________________________________package LogicalPro;

import java.util.ArrayList;

public class ConverBiToDesUsAL {

public static ArrayList<Integer> check(int num) {

ArrayList<Integer> a1= new ArrayList<Integer>();

	while(num>0)
{
	int rem=num%2;
		
	a1.add(rem);
		
	num=num/2;	
}
		
	for(int i=a1.size()-1; i>=0; i-- ) 
	{
        System.out.print(a1.get(i)+" ");
	}
		
	return a1;


	}
public static void main(String[] args) {

ConverBiToDesUsAL c1=new ConverBiToDesUsAL();

ConverBiToDesUsAL.check(38);
	}

}
_____________________________________________________________________________________________________________________
import java.util.Scanner;

public class AmstrongNum {

	static void test(int num)
	{
		int res=0;
		int temp=num;
		while(num>0)
		{
			int rem=num%10;
			res=res+(rem*rem*rem);
			num=num/10;
		}


		if(temp==res)
		{
			System.out.println(temp+" is Amstrong Numbers");
		}
		else
		{
			System.out.println(temp+" not Amstrong num");
		}


	}
	public static void main(String[] args) {
		Scanner sc =new Scanner(System.in);
		System.out.println("enter num");
		int num=sc.nextInt();
		test(num);

	}
}

_____________________________________________________________________________________________________________________
package LogicalPro;

public class ConvertDesToBin {
	public static int[] check(int num) {
		int i=0;
		int[] res= new int[10];
		while(num>0)	
		{
			int rem=num%2;
			res[i]=rem;
			num=num/2;
			i++;
		}
		for(int j=i-1; j>=0; j--)
		{
			System.out.print(res[j]+" ");
		}
		return res;
	}
	public static void main(String[] args) {

		check(25);
	}

}


_____________________________________________________________________________________________________________________
public class Factorial {

	static void test(int num)
	{
		int fact=1;
		int i=num;

		while(i>0)
		{
			fact=fact*i;
			i--;
		}
		System.out.println(fact);
	}

	public static void main(String[] args) {
		test(2);
	}
}
___________________________________________________________________________________________________________________

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

		test(year);
	}

}
_____________________________________________________________________________________________________________________

import java.util.Scanner;
public class PalandromString {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println(" enter String");
		String s=sc.nextLine();
		
		String rev="";	
		for(int i=s.length()-1; i>=0; i--)
		{
			rev=rev+s.charAt(i);
		}
		if(s.equals(rev))
		{
			System.out.println(" String is palindrom ");
		}
		else
		{
			System.out.println("String is not palindrom");
		}

	}

}
_____________________________________________________________________________________________________________________

public class PrimeNum {


	 static  void test(int n) {
		
		for(int i=2; i<=n; i++) 
			{
			int count=0;
			for(int j=2; j<i; j++) {
			if(i%j==0)
				{
					count++;
				}
			}
			if(count==0)
			{
				System.out.println(i+" ");
			}
			}
			}
		
	public static void main(String[] args) {
	System.out.println("main started");
	test(20);

	}

}
--------------------------------------------------------------------------------------------------------------------

public class ReverseString {
	public static void main(String[] args) 
	{
	String s="JAVA";
	char[] ch=s.toCharArray();
	

	for(int i=ch.length-1; i>=0; i-- )
	{
		System.out.print(" "+ch[i]);
	}
	}
	}
---------------------------------------------------------------------------------------------------------------------
		
 public class RoundSum {

	static int  round10(int n)
	{
		int rem=n%10;
		if(rem>=5)
		{
			n=n+(10-rem);
		}
		else
		{
			return n=n-rem;
		}
		return n;
	}
	static void test(int a, int b , int c)
	{
		System.out.println(round10(a)+ round10(b)+round10(c));
	} 
	public static void main(String[] args) {
		test(16,17,18);
	}
}
---------------------------------------------------------------------------------------------------------------------
import java.util.*;
public class SpyNumber 
{


	static void spy(int num)
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
	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		System.out.println(" enter num");
		int num=sc.nextInt();
		spy(num);

	}
}


---------------------------------------------------------------------------------------------------------------------
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
--------------------------------------------------------------------------------------------------------------------


public class ConBinToDes {
	
	
public static int binarytodecimal(String n) {
	    
	    String num=n;
	    int dec_value=0;
	    
	    int base=1;
	    int len=num.length();
	    for(int i=len-1; i>=0; i--)
	    {
	        if(num.charAt(i)=='1')
	        dec_value+=base;
	        base=base*2;
	    }
	    return dec_value;
	    
	    }
	    
	   public static void main(String[] args) {
		
		   String num = new String("1010");
		   System.out.println(binarytodecimal(num));
		   
		   
	   } 
	
---------------------------------------------------------------------------------------------------------------------	
package LogicalPro;

public class FibonacciS {

	static void testfib(int N)
	{
		int num1=0;
		int num2=1;

		int counter=0;

		while(counter<N)
		{
			System.out.print(num1+" ");
			int num3=num1+num2;

			num1=num2;
			num2=num3;
			counter=counter+1;
		}
	}
	public static void main(String[] args) {

		int N=10;

		testfib(N);


	}


}



_
