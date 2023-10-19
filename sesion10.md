<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Actividad10 -->
# Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.
Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno

# Solución
## Calcular la cantidad de materiales necesarios para construir una pared de ladrillos
Cálculo de la cantidad de materiales para la construcción: Este ejercicio consiste en calcular la cantidad de materiales necesarios para construir una estructura. Para ello, se debe tener en cuenta las dimensiones de la estructura y la cantidad de materiales necesarios por unidad de área o de volumen. Algunos ejemplos de cálculos de materiales son el cálculo de la cantidad de ladrillos necesarios para construir una pared, o el cálculo de la cantidad de concreto necesario para una losa o columna.

Ejemplo en Java de cómo calcular la cantidad de materiales necesarios para construir una pared de ladrillos:

```java
import java.util.Scanner;

public class CantidadLadrillos {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo;

      // Solicita las dimensiones de la pared
      System.out.print("Ingrese el largo de la pared en metros: ");
      largo = input.nextDouble();
      System.out.print("Ingrese el alto de la pared en metros: ");
      alto = input.nextDouble();
      System.out.print("Ingrese el ancho de la pared en metros: ");
      ancho = input.nextDouble();

      // Solicita las dimensiones del ladrillo
      System.out.print("Ingrese el largo del ladrillo en metros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en metros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en metros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      double areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}
```
## Explicacion del ejercicio de calcular la cantidad de materiales necesarios para construir una pared de ladrillos:

El ejercicio se centra en calcular la cantidad de ladrillos necesarios para construir una pared dada, teniendo en cuenta las dimensiones de la pared y los ladrillos. Aquí hay una explicación detallada: 
1. **Entrada de Dimensiones:** El programa comienza solicitando al usuario que ingrese las dimensiones de la pared en metros: largo, alto y ancho. - Luego, solicita las dimensiones del ladrillo: largoLadrillo, altoLadrillo y anchoLadrillo. 
2. **Cálculo de Áreas:**  Calcula el área de la pared (areaPared) multiplicando el largo por el alto. - Calcula el área de un ladrillo (areaLadrillo) multiplicando el largoLadrillo por el altoLadrillo. 
3. **Cálculo de la Cantidad de Ladrillos:** Utiliza la fórmula `cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo))` para determinar cuántos ladrillos son necesarios. - La fórmula divide el área de la pared entre el área de un ladrillo ajustada por el ancho de la pared y el ancho del ladrillo. La función `Math.ceil` redondea hacia arriba para asegurarse de que se comprendan suficientes ladrillos incluso si la división no es exacta.
 4. **Salida de Resultados**

## Calcular el movimiento rectilíneo uniforme
El movimiento rectilíneo uniforme (MRU) es un tipo de movimiento en el cual un objeto se mueve en línea recta y a velocidad constante, es decir, su velocidad no cambia en el tiempo. En este tipo de movimiento, la trayectoria del objeto es una línea recta, por lo que su aceleración es cero.

Un ejemplo común de MRU es un automóvil que se desplaza en una carretera recta y mantiene una velocidad constante durante todo el trayecto. Otro ejemplo es una pelota que cae verticalmente al suelo sin ser afectada por la resistencia del aire.

El MRU es un movimiento importante en la física, ya que permite entender conceptos básicos como la velocidad, la distancia recorrida y el tiempo de desplazamiento. Además, es utilizado como base para otros tipos de movimiento más complejos, como el movimiento rectilíneo uniformemente acelerado (MRUA) y el movimiento circular uniforme (MCU).

Ejemplo en Java de cómo calcular el movimiento rectilíneo uniforme:

```java
import java.util.Scanner;

public class MRU {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double velocidad, tiempo, distancia;
      
      // Solicita la velocidad y el tiempo
      System.out.print("Ingrese la velocidad en metros por segundo: ");
      velocidad = input.nextDouble();
      System.out.print("Ingrese el tiempo en segundos: ");
      tiempo = input.nextDouble();

      // Calcula la distancia recorrida
      distancia = velocidad * tiempo;

      // Muestra el resultado en la consola
      System.out.printf("La distancia recorrida es de %.2f metros.", distancia);
   }
}
```

## Explicación del ejercicio Movimiento rectilíneo uniforme
Para realizar realizar este ejercicio se se llevan acabo los sigientes puntos:

1. la creacion de un proyecto llama MRU lo cual indica movimiento rectilineo uniforme.(public class MRU , public static void main(String[] args) )
2. Crear un objeto de la clase Scanner llamado input el cual tomara los datos ingresados por el usuario( Scanner input = new Scanner(System.in);)
3. Se importa la libreria de Scanner( import java.util.Scanner;)
4. Se crean la variables velocidad, tiempo, distancia con el tipo de dato double.(double velocidad, tiempo, distancia;)
5. Se imprime un menseje al usuario indicando que ingresar en la variables de velocidad y tiempo.( System.out.print("Ingrese la velocidad en metros por segundo: "); velocidad = input.nextDouble(); System.out.print("Ingrese el tiempo en segundos: "); tiempo = input.nextDouble();)
6. En la variable distancia a tomar el resulatado de los datos ingresados por el usuario donde va a multiplicar la velocidad por el tiempo recorrido.( distancia = velocidad * tiempo;)
7. Se impreme el resultado en pantalla de la distancia recorrida en movimineto rectilineo uniforme( System.out.printf("La distancia recorrida es de %.2f metros.", distancia);).



