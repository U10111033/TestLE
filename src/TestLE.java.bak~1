/**U10111033, Computer science 4, Hsueh_Hsin Lu*/

import java.util.Scanner;

public class TestLE{
	public static void main(String[] args){
		Scanner input = new Scanner(System.in);
		
		System.out.println("Enter the coefficient 'a' of variable X in the first equation.");
		int a = input.nextInt();
		System.out.println("Enter the coefficient 'b' of variable Y in the first equation.");
		int b = input.nextInt();
		System.out.println("Enter the constant 'e' in the first equation.");
		int e = input.nextInt();
		System.out.println("Enter the coefficient 'c' of variable X in the second equation.");
		int c = input.nextInt();
		System.out.println("Enter the coefficient 'd' of variable Y in the second equation.");
		int d = input.nextInt();
		System.out.println("Enter the constant 'f' in the second equation.");
		int f = input.nextInt();
		
		LinearEquation myLE = new LinearEquation(a, b, c, d, e, f);
		
		if(!myLE.isSolvable()){
			System.out.println("The equation has no solution.");
		}else{
			System.out.println("Result is : X = " + myLE.getX() + " Y = " + myLE.getY());
		}
	}
}

class LinearEquation {
	private double a, b, c, d, e, f;
	LinearEquation(){
		
	}
	
	LinearEquation(double a, double b, double c, double d, double e, double f){
		this.a= a;
		this.b= b;
		this.c= c;
		this.d= d;
		this.e= e;
		this.f= f;
	}
	
	double getA(){
		return a;
	}
	
	double getB(){
		return b;
	}
	
	double getC(){
		return c;
	}
	
	double getD(){
		return d;
	} 
	
	double getE(){
		return e;
	}
	
	double getF(){
		return f;
	}
	
	boolean isSolvable(){
		return !(a*d - b*c == 0);
	}
	
	double getX(){
		if(!isSolvable()){
			System.out.println("Error, not sovable.");
			return 0;
		}else
			return (e*d-b*f)/(a*d-b*c);
	}
	
	double getY(){
		if(!isSolvable()){
			//System.out.println("Error, not sovable.");
			return 0;
		}else
			return (a*f-e*c)/(a*d-b*c);
	}
}