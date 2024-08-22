# java-programs
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
