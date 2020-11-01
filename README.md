# Programa-en-C
Ejercicio resuelto y comentado con explicación
Escriba un programa que introduzca un número de cinco dígitos, que separe el número en sus dígitos individuales
y que despliegue los dígitos separados entre sí mediante tres espacios cada uno. 
Pista: Utilice combinaciones de la división entera y el operador módulo.
Por ejemplo, sí el usuario escribe 42138 el programa debe imprimir. 

4      2     1     3     9 

<script src="//onlinegdb.com/embed/js/Hkengho_P?theme=dark"></script>

https://onlinegdb.com/rkRn3oodP


/******************************************************************************

Welcome to GDB Online.
GDB online is an online compiler and debugger tool for C, C++, Python, PHP, Ruby, 
C#, VB, Perl, Swift, Prolog, Javascript, Pascal, HTML, CSS, JS
Code, Compile, Run and Debug online from anywhere in world.

*******************************************************************************/

#include <stdio.h>

int main()
{
    /* crea la variable número, de tipo entero */
    int number, a, b, c, d, e, f;
    
    //El \n al final indica nueva salto de línea.
  printf( "Escriba un número de 5 dígitos: \n" ); 
  
  /*Por ejemplo, %d le dice a printf () que imprima un número entero.
    &variable - define la variable de referencia. 
  */
  /*
    Se escanea un dato de entrada con scanf, de tipo entero
  */
  scanf( "%d", &number );
	
  a = number; //Se asigna el 42139
  //42139 / 10000 = 4,2139 se toma el entero 4.
  b = a / 10000;
  //42139 / 1000 módulo 10, da como resultado 2.
  c = a / 1000 % 10; 
  //42139 / 100 módulo 10, da como resultado 1.
  d = a / 100 % 10;
  //42139 / 10 módulo 10, da como resultado 3.
  e = a / 10 % 10;  
  //42139 módulo 10, da como resultado 9.
  f = a % 10; 

//%d También define los espacios donde se colocarán los números enteros. 
  printf( "%d   %d   %d   %d   %d\n", b, c, d, e, f );
}
	https://miniwebtool.com/es/modulo-calculator/ 


