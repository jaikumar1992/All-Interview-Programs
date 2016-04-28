# All-Interview-Programs

public class Armstrongno {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
	int i,k,t=0;
	Scanner scan=new Scanner(System.in);
	System.out.println("pls enter to find");
	i=scan.nextInt();
	int temp =i;
	while(0<i){
		k=i%10;
		i=i/10;
		t=t+(k*k*k);
	}
	if(temp==t)
	System.out.println("true");
	else
		System.out.println("false");
	}
	}
---------------------------------------------------------------------



public class Fib {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
int n=0,n1=1,m,p;
Scanner scan=new Scanner(System.in);
m=scan.nextInt();
System.out.println(n+" \n"+n1);
for(int i=0;i<m;i++){
	p=n+n1;
	System.out.println(" "+p);
	n=n1;
	n1=p;
}

	}

}
-------------------------------------------------

public class Checkprime {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
int count=0;
		Scanner scan=new Scanner(System.in);
System.out.println("enter he no to find");
int no=scan.nextInt();
	for(int i=2;i<no;i++){
		if(no%i==0){
			count++;
			break;
		}
	}
	if(count==0){
		System.out.println("true");
	}
	else{
		System.out.println("false");
	}
	}
}
------------------------------------------------------


public class Reversestring {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
String original,reverse="";
		Scanner scan=new Scanner(System.in);
System.out.println("enter the name to reverse");
original=scan.nextLine();
//int length=original.length();
//for(int i=length-1;i>=0;i--){
//	reverse=reverse+original.charAt(i);
	int length=original.length();
	for(int i=length-1;i>=0;i--){
		reverse=reverse+original.charAt(i);
}
System.out.println(reverse);
	}

}
----------------------------------------------


public class Stringreplace {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
Scanner scan=new Scanner(System.in);
System.out.println("enter some words to find");
String s=scan.nextLine();
	//	String s="my name is jaikumar";
//System.out.println(s);
String str=s.replaceAll("[aeiou]", "");
System.out.print(str);
String [] s1=str.split("\\s");
for(String st:s1){
	System.out.println(st);
}
	}

}
--------------------------------------------------------

public class Equalstring {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
String str="jai";
String str1="Jai";
System.out.println(str.compareTo(str1));
if(str.equalsIgnoreCase(str1))
	System.out.println("both are not equal");
else
	System.out.println("both are equal");
	
	if(str.equals(str1))
		System.out.println("both are not equal");
	else
		System.out.println("both are equal");
}}
-----------------------------------------------------
public class Factorial {

	void fact(){
		Scanner scan=new Scanner(System.in);
		System.out.println("enter the number");
		int no=scan.nextInt();
	int fact=1;
	for(int c=no;c>0;c--){
		fact=fact*c;
	}
	System.out.println(fact);
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub

Factorial f=new Factorial();
f.fact();
	}

}
-------------------------------------------------

public class Patern {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scan=new Scanner(System.in);
		System.out.println("enter number");
		int no=scan.nextInt();
		for(int i=0;i<no;i++){
			for(int j=0;j<no-i;j++){
				System.out.print(" ");
			}
			for(int k=0;k<=i;k++){
				System.out.print("  *");
			}
			System.out.println("");
		}
	}

}
--------------------------------------


public class Swapping2no {

static int a,b,temp;
public void swap(){
	temp=a;
	a=b;
	b=temp;
	System.out.println(a);
	System.out.println(b);
}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Swapping2no s=new Swapping2no();
		Scanner scan=new Scanner(System.in);
	System.out.println("enter the first no");
		a=scan.nextInt();
		System.out.println("enter the seond no");
		b=scan.nextInt();
		System.out.println("swapped now");
		s.swap();
	}

}
-------------------------------------------------



package com.java.Programs;

import java.util.Scanner;

public class ReverseNo {
	
	public void reverse(){
		Scanner scan=new Scanner(System.in);
		System.out.println("Please enter your number");
		int a=scan.nextInt();
		do{
			int b=a%10;
			System.out.print(b);
			a=a/10;
		}while(a>0);
		
		}
	
	public static void main(String[] args) {
		// TODO Auto-generated method stub
     //	ReverseString rs=new ReverseString();
		//		rs.reverse();
				ReverseNo rn=new ReverseNo();
				rn.reverse();
			}

		

	}


------------------------------------------


package com.java.Programs;

import java.util.Scanner;

public class OddorEven {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
Scanner scan=new Scanner(System.in);
System.out.println("enter the number to find");
int a=scan.nextInt();
if(a%2==0)
	System.out.println("your number is even number");
else
	System.out.println("your number is odd number");
	}

}
