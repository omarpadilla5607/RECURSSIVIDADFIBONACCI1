# RECURSSIVIDADFIBONACCI1
La sucesión comienza con los números 0 y 1,2​ y a partir de estos, «cada término es la suma de los dos anteriores», es la relación de recurrencia que la define.

codigo java 

package calculofobonacci;
public class CalculoFobonacci {
// declaración recursiva del método fibonacci
 public long fibonacci( long numero )
 {
 if ( ( numero == 0 ) || ( numero == 1 ) ) // casos base
 return numero;
 else // paso recursivo
 return fibonacci( numero - 1 ) + fibonacci( numero - 2 );
 } // fin del método fibonacci

 public void mostrarFibonacci()
 {
 for ( int contador = 0; contador <= 16; contador++ )
 System.out.printf( "Fibonacci de %d es: %d\n", contador,
 fibonacci( contador ) );
 } // fin del método mostrarFibonacci
 } // fin de la clase CalculoFibonacci 
 
 
Metodo Fibonacci
package calculofobonacci;
public class PruebaFibonacci {
    public static void main( String args[] )
 {
 CalculoFobonacci calculoFibonacci = new CalculoFobonacci ();
 calculoFibonacci.mostrarFibonacci();
 } // fin de main
 } // fin de la clase PruebaFibonacci
