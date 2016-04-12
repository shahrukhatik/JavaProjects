Description: This application will be used to convert a user given volume in cups to its equivalent number of teaspoons, tablespoons, ounces, pint, quarts, or gallons. 

    import java.lang.*;
    import java.util.*;

    /* 
    	Date: 1st February 2016

    	This program will allow us to view what a certain volume of cups would be in
    	tablespoons, teaspoons etc.
	
    	This program will need the number of cups from the user.
    	Then the program will output the neccessary teaspoons, tablespoons etc.
	
	                    4 cups equals 4 * 48 = 192 teaspoons
	                    4 cups equals 4 * 16 =  64 tablespoons
	                    4 cups equals 4 * 8   =  32 ounces
	                    4 cups equals 4 * 0.5   =  2 pints
	                    4 cups equals 4 * 0.25   =  1 quart
	                    4 cups equals 4 * 0.0625   =   0.2500 gallon
						
    	java.util and java.text will be used
	
    	The input and output will be simple text based interactions using 
    	system.out.Println and scanner
	
    	Psuedocode: 
				Output a welcome message
				Output a message that describes what the program will do
				Output a message requesting the number cups the user wishes to 
				convert
				
				read the input value and store it
				
				calculate the teaspoons, tablespoons etc and store it.
				
				output a message that displays this values so the user can see
				it
    */

    class cupsconversion
    {

    public static void main(String[] args)
    {
    	System.out.println("Welcome to Shahrukhs Cup Conversion Program");
    	System.out.println();
    	System.out.println("This application will be used to convert a user given volume");
    	System.out.println("in cups to its equivalent number of teaspoons, tablespoons, ounces, pints");
    	System.out.println("quarts, or gallons");
    	System.out.println("\n \n");
    	System.out.println("Please type in a +ve real value for the number of cups you want converted");
    	System.out.print(" Number of cups = ");
	
    	Scanner input = new Scanner(System.in);
	
    	float cups; // We are storing the input the user puts in float.
	
    	cups = input.nextFloat(); // read and convert user input and store it

    	float teaspoons = cups * 48;
	
    	float tablespoons = cups * 16;
	
    	float ounces = cups * 8;
	
    	float pints = cups * 0.5f; // have to add f for java to caclulate this correctly.
	
    	float quarts = cups * 0.25f;
	
    	float gallons = cups * 0.0625f;
	
    	System.out.println(" Given " + cups + " cups, the volume in teaspoons are " + teaspoons);
    	System.out.println(" Given " + cups + " cups, the volume in tablespoons are " + tablespoons);
    	System.out.println(" Given " + cups + " cups, the volume in ounces are " + ounces);	
    	System.out.println(" Given " + cups + " cups, the volume in pints are " + pints);	
    	System.out.println(" Given " + cups + " cups, the volume in quarts are " + quarts);
    	System.out.println(" Given " + cups + " cups, the volume in gallons are " + gallons);
	
    }

    }
