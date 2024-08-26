# java-programs
# Arithmetic Exception
package exceptions;
public class Ex2 {
public static void main(String[] args) {
		// TODO Auto-generated method stub
		try
		{
		Student s =new Student();
		 s.display();
		}
		catch (ArithmeticException e)
		{
			System.out.println("Exception caught");
		}
	}

}
class Student
{
	void display() throws ArithmeticException
	{
		System.out.println(2/0);
	}
}

#Exception Handling
package exceptions;
import java.util.Scanner;
public class Ex1 {
public static void main(String[] args) {
		// TODO Auto-generated method stub
	   try
	   {
       Scanner sc= new Scanner(System.in);
       int n1 = sc.nextInt();
       int n2 = sc.nextInt();
       if(n2==2) 
       {
    	   throw new sindhuException("Exception thrown by sindhu");
       }
       System.out.println(n1/n2);
       sc.close();
	   }
	   catch(sindhuException e) {
		   System.out.println(e.getMessage());
	   }
	   catch(Exception e) {
		   System.out.println("all exceptions are caught");
		   
	   }
	   
	}

}
class sindhuException extends Exception
{
	sindhuException(String str)
	{
		super(str);
	}
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#prime number
import java.util.Scanner;
public class P10 {
public static void main(String[] args) {
	// TODO Auto-generated method stub
	Scanner sc=new Scanner(System.in);
	system.out.println("x:");
	int x=sc.nextInt();
	boolean flag=false;
	for(int i=2;i<=x/2;++i)
	  {
		if(x%i==0) {
			flag=true;
			break;
		}
	 }
	if(!flag)
        {
		System.out.println("it is prime");
	}
	else
	{
		System.out.println("it is not prime");
	}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 # asci value
 package arrays;

 public class Asci {
     public static void main(String[] args) {
		// TODO Auto-generated method stub
		int ascii[]= {90,63,64,111,118,101,32,93};
		for(int i=0;i<ascii.length;i++)
		{
			System.out.println((char)ascii[i]+" ");
		}
        System.out.println();
	}

}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# search an element
package arrays;

public class Check {
	public static void main(String[] args)
	{
		int x[]= {10,20,30,40,50};
		int needed=30;
		int index=-1;
		for(int i=0;i<x.length;i++) {
			if(x[i]==needed)
			{
				System.out.println( "3");
				index=index+1;
			}
			else
			{
				System.out.println(" -1");
			}
			
		}
	}

}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# sorting element
package arrays;
import java.util.Arrays;

public class Sorted {
public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a []= new int[]{10,50,30,20,40};
		Arrays.sort(a);
		System.out.println("Elements of array sorted in ascending order:");
		for(int i=0;i<a.length;i++) {
			System.out.println(a[i]+" ");
		}
		

	}

}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# sum and average
package arrays;

public class Sum {
public static void main(String[] args) {
		// TODO Auto-generated method stub
		int x[]=new int[] {10,20,30};
		int sum=0;
		for(int i=0;i<x.length;i++) {
			sum=sum+x[i];
		}
		System.out.println(sum);
		float Average=0;
		Average=sum/3;
		System.out.println(Average);

	}

}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# maximum value
package arrays;

public class Max {
public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]={10,20,30};
		System.out.println(a[0]);
		System.out.println(a[a.length-1]);
		

	}

}
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------# Java program for simple calculator
import java.io.*;
import java.lang.*;
import java.lang.Math;
import java.util.Scanner;

// Driver class
public class BasicCalculator {
	// main function
	public static void main(String[] args)
	{
		// Stores two numbers
		double num1, num2;

		// Take input from the user
		Scanner sc = new Scanner(System.in);

		System.out.println("Enter the numbers:");

		// Take the inputs
		num1 = sc.nextDouble();
		num2 = sc.nextDouble();

		System.out.println("Enter the operator (+,-,*,/):");

		char op = sc.next().charAt(0);
		double o = 0;

		switch (op) {
		// case to add two numbers
		case '+':
			o = num1 + num2;
			break;

		// case to subtract two numbers
		case '-':
			o = num1 - num2;
			break;

		// case to multiply two numbers
		case '*':
			o = num1 * num2;
			break;

		// case to divide two numbers
		case '/':
			o = num1 / num2;
			break;

		default:
			System.out.println("You enter wrong input");
		}

		System.out.println("The final result:");
		System.out.println();

		// print the final result
		System.out.println(num1 + " " + op + " " + num2
						+ " = " + o);
	}
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
