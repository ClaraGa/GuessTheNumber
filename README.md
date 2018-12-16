# GuessTheNumber
package lab2;

import java.util.Scanner;

public class GissaTal {

	
	public static void main(String[] args) {
		
		System.out.print("Mata in ett heltal mellan 0 och 100: ");
		Scanner input = new Scanner(System.in);
		int rättTal = input.nextInt();
		
		int antal_rader = 5;
		
		for(int i = 0; i<antal_rader; i++) {
			System.out.println('\n');
		}
		
		System.out.print("Mata in ett heltal mellan 0 och 100, som du tror är samma som din kompis heltal: ");
		int gissatTal = input.nextInt();
		
		int antal_gissningar = 1;
		
		
		while (gissatTal != rättTal){
		
	
			if (gissatTal < rättTal){
				System.out.println("FEEL ditt tal är mindre än det korrekta talet :( Gissa igen: ");
			
				gissatTal = input.nextInt();
				
			}
			
			else if (gissatTal > rättTal){
				System.out.println("FEEL ditt tal är större än det korrekta talet :( Gissa igen: ");
			
				gissatTal = input.nextInt();
				
			}
		
			antal_gissningar ++;
	
		}
		
		System.out.println("Grattis!! Du är grym för du gissa rätt tal bland 100 möjliga!!!:)))" + "Du gissade " + antal_gissningar + " gånger.");
			
	}
}
