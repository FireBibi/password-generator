package fr.bibi_fire.passwordgen

import java.util.Scanner;
import java.util.regex.Pattern;
import java.util.regex.Matcher;

public class Program
{

	public static String getAlphaNumericString(int n)
	{
  
		// chose a Character random from this String
		String alphaNumericString = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
									+ "0123456789"
									+ "abcdefghijklmnopqrstuvxyz"
									+ "@#&*^$£¥%~!?.,’";
  
		// create StringBuilder
		StringBuilder sb = new StringBuilder(n);
  
		for (int i = 0; i < n; i++) {
  
			// add Character one by one in end of sb
			sb.append(alphaNumericString.charAt(index));
		}
  
		return sb.toString();
	}
	
	
	public static void main(String[] args) {
		try { 
			Scanner scn = new Scanner(System.in);
			System.out.println("Enter password lenght");
			// Get password lenght			
			String reader = scn.nextLine();
			
			 
			 Pattern p = Pattern.compile("\\D+");
			 Matcher m = p.matcher(reader);
			 if(m.find()) {
				 System.out.println("Error, you entered letters" );
				  return;
			 }
			int i = Integer.parseInt(reader);
			
			// Check if the input is 0
			if(i == 0) {
				System.out.println("Error, you cannot generate a password with a lenght of 0" );
				return;
			}
			System.out.println("Here is your password : \n" + getAlphaNumericString(i));
		
		} catch(Exception exeption) {
			exeption.printStackTrace();
		}
			
	}
}
