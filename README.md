import java.util.Scanner;
class School{

	void display(String name, int roll){
		System.out.println("Name :" + name);
		System.out.println("Roll :" + roll);

	}


	int calculate(int m1,int m2,int m3){

		int totalMarks;
		totalMarks= m1+m2+m3;

		return totalMarks;
	}

	}




public class Student1 {

	public static void main(String args[]){

		int roll, m1, m2, m3;
		String name;				//declaration

		School obj= new School(); 		//instance creation
                Scanner i = new Scanner(System.in);
		

		for( int count=1;count<=3;count++){      

		

			
			System.out.println("Student "+ count+ " Details" );
			System.out.println("==================");
			
			System.out.println("Enter name");

			name = i.next();			

			System.out.println("Enter roll");

			roll = i.nextInt();
		
			System.out.println("Enter m1");

			m1 = i.nextInt();

			System.out.println("Enter m2");

			m2 = i.nextInt();

			System.out.println("Enter m3");
		
			m3 = i.nextInt();

			
			System.out.println("Student Details");
			
			System.out.println("================");
			
			obj.display(name,roll);

			System.out.println("Total mark: "+ obj.calculate(m1,m2,m3));
			
			System.out.println();
			
		}

	}
}
