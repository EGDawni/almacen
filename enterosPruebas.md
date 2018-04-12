# almacen
package pruebas;

import java.util.InputMismatchException;
import java.util.Scanner;

public class prueba_entero {
	public static void main(String[]args){
		int a;
		boolean repetir=false;
		Scanner sc=new Scanner(System.in);
		do{
		try{
			repetir=false;
			System.out.println("Introduce un numero entero: ");
			a=sc.nextInt();
			System.out.println("Numero leido es: "+a);
		}catch(InputMismatchException e){
			System.out.println("Debe introducir un numero entero.");
			System.out.println(e);
			repetir=true;
			sc.nextLine();
		}
		}while(repetir);
	}
}
