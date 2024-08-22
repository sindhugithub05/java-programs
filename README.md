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
