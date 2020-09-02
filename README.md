# complex.java
https://github.com/sarveshashelar/complex.git
// User defined Complex Class
public class Complex {
	
	// Declaring variables
	int real, imaginary;
	// User defined Complex Class
public class Complex {
	
	// Declaring variables
	int real, imaginary;
	
	//Empty constructor
	Complex()
	{
	}
	//Constructor to accept
	//real and imaginary part
	Complex(int tempReal, int tempImaginary)
	{
		real = tempReal;
		imaginary = tempImaginary;
	}
	//Constructor to accept
    //real and imaginary part
	Complex addComp(Complex C1, Complex C2)
	{
		// creating temporary variable
		Complex temp = new Complex();
		
		// adding real part of complex numbers
		temp.real = C1.real + C2.real;
		
		// adding imaginary part of complex numbers
		temp.imaginary = C1.imaginary + C2.imaginary;
		
		//returning the sum
		return temp;
	}
	
	
	
	
	
	
	// function for printing complex number
	void printComplexNumber()
	{
		System.out.println("Sum of complex number:" 
	                       + real + "+" + imaginary + "i");
	}
	
	
// MainClass 

public static void main(String[] args)
{
	// First Complex number
		
	Complex C1 = new Complex(3,2);
		
	// printing first complex number
	C1.printComplexNumber();
		
	// Second Complex number
		
	Complex C2 = new Complex(9,5);
			
	// printing first complex number
	C2.printComplexNumber();
			
	// for Storing the sum
	Complex C3 = new Complex();
			
	// calling addComp() method
	C3 = C3.addComp(C1, C2);
			
	// print the sum
			
	C3.printComplexNumber();

	}
} 
