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




 

