<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->
# Actividad 3: Ejercicios de operaciones básicas en Java.
1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

# Solución
1. 
``` java
import java.util.Scanner;
class Main {
  public static void main(String[] args) {
    Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero:");
        int num1 = entradaDatos.nextInt();

        System.out.println("Ingrese el segundo numero:");
        int num2 = entradaDatos.nextInt();

        int suma = num1 + num2;
        int multiplicacion = num1 * num2;

        System.out.println("El resultado de la suma de los dos numeros es: " + suma);
        System.out.println("El resultado de la multipliccion de los dos numeros es: " + multiplicacion);
  }
} 
```
2. 
``` java
import java.util.Scanner;
public static void main (String[] args) {
   Scanner entradaDatos = new Scanner (source: System.in);
 
       System.out.printIn (w: "Ingrese el primer numero");
       int num1 = entradaDatos.nextInt () ;

       System.out.printIn (x: "Ingrese el segundo numero");
       int num2 = entradaDatos.nextInt () ;
       
       int Resta = num1 - num2;
       int Division = num1 / num2;

       System. out.printin ("El resultado de la suma de los dos numeros es: " + Resta);
       System. out.printIn ("EL resultado de la multiplicacion de los dos numeros es: " + Division);
 }
```
3. 
``` java
import java.util.Scanner;
public static void main (String[] args) {
  Scanner entradaDatos = new Scanner (source: System.in);

      System.out.printIn(a: "Ingrese el primer numero entero");
      int num1 = entradaDatos. nextInt () ;

     System.out.println (x:"Ingrese el segundo numero entero");
     int num2 = entradaDatos. nextInt () ;

     System.out.printin (r: "Ingrese el tercer numero entero");
     int num3 = entradaDatos.nextInt () ;

     int suma = num1 + num2 + num3;
     int multiplicacion = numl * num2;
     int division = numl * num2 / num3;

     System.out.printin ("la suma de los tres numeros es:
" + suma);
     System.out.print]n ("la multiplicacion de los dos numeros es: " + multiplicacion);
     System.out.printin ("El resultado de los dos numeros dividido por el tercer numero es: " + division);
 }
```
4. 
``` java
import java.util.Scanner;
public static void main (String[] args) {
  Scanner entradaDatos = new Scanner (source: System.in) ;

      System.out.printIn (x: "Ingrese el primer numero decimal");
      float numl = entradaDatos.nextFloat () ;

      System.out.printin (x: "Ingrese el segundo numero decimal");
      float num2 = entradaDatos. nexFloat () ;

      float suma = numl + num2;
      float resta = num1 - num2;
      float multiplicacion = num1 * num2;
      float division = numl / num2;
      
      System.out.printIn ("El resultado de la suma es: " + suma);
      System.out.printIn ("El resultado de la resta es:
" + resta);
      System.out.printIn ("El resultado de la multiplicacion es: " + multiplicacion);
      System.out.printIn ("El resultado de la division es:
" + division);
 }
```
5. 
``` java
import java.util.Scanner;
public static void main (String[] args) {

    int numero = 35;
    int suma = 35 + 1;
    int resta = 35 - 1;

    System.out.printin ("El incremento es: + suma);
    System.out.printin ("El decremento es: - resta);
 }
```
6. 
``` java
import java.util.Scanner;
public class Ejercicio_06 {
  public static void main (String[] args) {

    int numero = 24;
    int suma = 24 + 5;
    
    System.out.printin ("El resultado de la asignacion compuesta es: " + suma);
 }
}
```
7. 
```java 
import java.util.Scanner;
public static void main (String[] args) {
    Scanner entradaDatos = new Scanner (source: System.in);

    boolean mayordeEdad = true;
    
    System.out.println (x: "Ingreso a la discoteca");

    System.out.println (x: "Por favor ingrese su estatura");
    int estatura = entradaDatos.nextInt () ;

    System.out.println (x: "Por favor ingresa su edad");
    int edad = entradaDatos.nextInt () ;

    boolean ingresoDiscoteca = ( (edad>=18) && (estatura>=1.55) | | (mayordeEdad) ) ;

    System.out.printin ("Resultado de ingreso a la discoteca es: " + ingresoDiscoteca);
 }
 ```
8. 
```java
import java.util.Scanner; 
public class ejercicio 08 {
  public static void main (String [] args) {
    Scanner entradaDatos = new Scanner (source: System.in);

    System.out.printin (x: "Por favor ingresa un numero");
    int numero = entradaDatos.nextInt () ;
    
    if (numero == 0) {
       System.out.printin (x: "el numero es neutro");
}
    else if (numero‹=0) (System.out.printin (x: "el numero es negativo");
   }else { System.out.println (x: "el numero es positivo"); }

  }

 ```





