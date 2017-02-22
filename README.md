# Assignment-3.6
1) Can you overload a method with same return type.? Explain your answer with proper logic.
Ans:  Yes,we can overload a method with same return type. Here two methods with
   same name are created and return type of both is string we have succesfully 
   overloaded the methods with same return type.

    import java.util.Scanner;
    public class acad {
  	public static String string(String a , String b)
    {
		String s=a+" "+b;
		return s;
    }
    public static String string(String c)  
    {
    	String s1=c;
         return c;
    }
	
	  public static void main(String args[])
	  {
		Scanner sc= new Scanner(System.in);
		
		String a = sc.nextLine();
		String b= sc.nextLine();
		String c="Angel";
		System.out.println("String");
		System.out.println(string(a,b)); //2 String as input
		System.out.println(string(c));   //1 String as input
		}
	  }

2) Write a program in java using Arrays, that sorts the element in descending order.
Ans: 
import java.util.Arrays;
import java.util.Scanner;

public class acad {
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int n=sc.nextInt(); //size of array
int[] a=new int[n]; // declaration of array
for(int i=0;i<n;i++){
a[i]=sc.nextInt();
}
Arrays.sort(a);               //sorting of array
for(int i=a.length-1;i>=0;i--){
System.out.println(a[i]+" "); // displaying sorted reverse ordered array elements
}
}
}
