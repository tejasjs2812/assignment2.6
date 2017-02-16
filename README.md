# assignment2.6


Que.A)
import java.util.Scanner;

public class acad2 {
	
public static void main(String args[])
{
	StringBuffer sb = new StringBuffer();    //initiate buffer to store even values
		StringBuffer sb1 = new StringBuffer();//initiate buffer to store odd values
		Scanner sc =new Scanner(System.in); //scan input from user
		int a = sc.nextInt();  //declare variable and scan value from user
		int b =sc.nextInt();   //declare variable and scan value from user
		for (int i = a; i <=b; i++) { // run loop within range of input
			if(i%2==0) //check if number is even
			{
				sb.append(i);
				sb.append(" "); //store in buffer sb
			}
			else
			{
				sb1.append(i);
				sb1.append(" "); //if odd store in buffer sb1
			}
		}
		System.out.println("The even number are"); //print values in buffer sb
		System.out.println(sb.toString());
		System.out.println("The odd number are"); //print values in buffer sb2
		System.out.println(sb1.toString());
	}

}
Que.B)

import java.util.Scanner;

public class acad2 {
	
public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in); // to scan input from user 
		System.out.println("Input"); //print input 
		int no = sc.nextInt();       //scan value from user to print multiples
		System.out.println("Output"); 
		for (int i = 1; i <=10; i++) {
			System.out.println(no+"x"+i+"="+i*no); //print 10 multiples of no
			
		}
	}

}

Que.C)

Method Overloading-
If a class has multiple methods having same name but different in parameters, it is known as Method Overloading.
it can be done be achieved by either changing data type or changing number of argument. 
 Lets see by exanple 
 1. Changing data type- here method named sum is used to perform addition of int type as well as string type of inputs. 
 method performs the same action without errors
 
 import java.util.Scanner;
public class acad2 {
	public static void sum(int a , int b) //create method sum sum two int
    {
         System.out.println(a+b);
         
    }
    public static void  sum(String s ,String s1) //another method named sum for string
    {
    	String s4 = s+s1;
         System.out.println(s4);
    }
	
	public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		int a = sc.nextInt(); //scan input a as int
		int b = sc.nextInt(); //scan input b as int
		String st = sc.next(); //scan input st as string
		String st1 = sc.next(); //scam input st1 as string
		sum(a,b);//sum with integer type as input
		sum(st,st1);//	sum with String type as input
		}
	}
  2.by changing number of arguments-here we passed two arguments to perform then changed it to three,
  the method run without errors.
  
  import java.util.Scanner;
class acad2{  
static int add(int a,int b){return a+b;}   //pass two arguments to operate on..case1
static int add(int a,int b,int c){return a+b+c;}//change no. of arguments passed..case1
public static void main(String[] args){  
System.out.println(acad2.add(11,15));  //print sum for case1
System.out.println(acad2.add(11,15,19));  //print sum for case2
}}  
