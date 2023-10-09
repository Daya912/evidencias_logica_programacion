<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Actividad 07 -->

# Actividad: Ejecicios Array - ArrayList
## 1. En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList

### Ejemplo Array
```java
import java.util.Arrays;

public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
```
### Ejemplo Array list
```java 
import java.util.ArrayList; 
import java.util.Scanner;

public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }

  public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}
```
## 2. Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.

## Solución 
## Array
1.  Se crea un array de números enteros llamado "numeros" e inicializado con los valores 5, 2, 10, 7, 1.

2. Imprime el array original usando Arrays.toString() para obtener una representación legible del array.

3. Calcula la suma de todos los elementos en el array mediante un bucle for.

4. Encuentra el número más grande en el array mediante un bucle for y una variable (maximo) que se actualiza si se encuentra un número mayor.

5. Utiliza el método sort de la clase Arrays para ordenar el array en orden ascendente y luego imprime el array ordenado.

En resumen, este programa realiza operaciones básicas con un array de números enteros, como imprimir el array original, calcular la suma de sus elementos, encontrar el número más grande y ordenar el array en orden ascendente.

## ArrayList

1. Se utiliza un ArrayList llamado notas para almacenar las notas. A diferencia de un array tradicional, un ArrayList puede cambiar de tamaño dinámicamente.

2. Se utiliza un objeto Scanner para obtener la entrada del usuario.

3. Se implementa un bucle while(true) para mostrar un menú continuo hasta que el usuario elija salir (opción 3).

4. La opción 1 permite al usuario agregar una nueva nota llamando al método agregarNota.

5. La opción 2 permite al usuario mostrar todas las notas llamando al método mostrarNotas.

6. El programa usa métodos separados (agregarNota y mostrarNotas) para organizar el código y hacerlo más modular y fácil de entender.

7. En el método agregarNota, se solicita al usuario que ingrese el título y el contenido de la nota, y luego se agrega al ArrayList.

8. En el método mostrarNotas, se itera a través del ArrayList e imprime cada nota en la consola.

## 2.
## Array 
```java
public class EjemploArray {

    public static void main(String[] args) {
        // Declarar un array de enteros
        int[] numeros = new int[5];

        // Asignar valores al array
        numeros[0] = 10;
        numeros[1] = 20;
        numeros[2] = 30;
        numeros[3] = 40;
        numeros[4] = 50;

        // Imprimir el contenido del array
        System.out.print("Contenido del array: ");
        for (int i = 0; i < numeros.length; i++) {
            System.out.print(numeros[i] + " ");
        }

        // Calcular y imprimir la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("\nSuma de los elementos: " + suma);
    }
}
```
Este programa crea un array de enteros llamado numeros con una longitud de 5. Luego, asigna valores a cada elemento del array y los imprime. Finalmente, calcula la suma de los elementos del array y la imprime.

## ArrayList
```java
import java.util.ArrayList;

public class EjemploArrayList {

    public static void main(String[] args) {
        // Crear un ArrayList de cadenas (Strings)
        ArrayList<String> nombres = new ArrayList<>();

        // Agregar elementos al ArrayList
        nombres.add("Juan");
        nombres.add("María");
        nombres.add("Carlos");
        nombres.add("Ana");

        // Imprimir el contenido del ArrayList
        System.out.println("Contenido del ArrayList: " + nombres);

        // Obtener y modificar un elemento del ArrayList
        String nombreAntiguo = nombres.get(2);
        nombres.set(2, "Pedro");

        // Imprimir el ArrayList después de la modificación
        System.out.println("ArrayList después de la modificación: " + nombres);

        // Obtener la longitud del ArrayList
        int longitud = nombres.size();
        System.out.println("Longitud del ArrayList: " + longitud);

        // Verificar si el ArrayList contiene un elemento específico
        boolean contieneCarlos = nombres.contains("Carlos");
        System.out.println("¿Contiene 'Carlos'? " + contieneCarlos);

        // Eliminar un elemento del ArrayList
        nombres.remove("María");

        // Imprimir el ArrayList después de la eliminación
        System.out.println("ArrayList después de la eliminación: " + nombres);
    }
}
```

Este programa crea un ArrayList llamado nombres que almacena cadenas (Strings). Agrega elementos, imprime el contenido, modifica un elemento, muestra la longitud del ArrayList, verifica si contiene un elemento específico, y finalmente elimina un elemento y muestra el estado final del ArrayList.



















