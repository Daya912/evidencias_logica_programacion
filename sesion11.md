<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


<!-- Actividad 11 -->
# Actividad: Ejercicios de Lógica de Programación
1. Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

2. Desarrollar un algoritmo que realice la conversión de binario a decimal.

# Solución
### 1. 
```java
package com.mycompany.ejerciciosesion11_1;

import java.util.HashSet;
import java.util.Set;

public class EjercicioSesion11_1 {

    public static void main(String[] args) {
      int[] numeros = {1, 2, 3, 4, 5, 2,4,5,3,7,12,12,7};

        // Creamos un hashSet para almacenar los numeros repetidos.
        Set<Integer>numerosRepetidos = new HashSet<>();

        // Recorremos el conjunto de números
        for (int i = 0; i < numeros.length; i++) {
            System.out.println("numeros en i" +numeros[i]);
            for (int j = 0; j < i; j++) {
                System.out.println("numeros en j"+numeros[j]);
                if (numeros[i] == numeros[j]) {
                    // El número actual ya ha aparecido
                    numerosRepetidos.add(numeros[i]);
                }
            }
        }

        System.out.println("Los numero repetidos son:"+ numerosRepetidos);
    }
} 
```

### 2.
```java
public class Main {
    public static void main(String[] args) {
        String binario = "100101";
        int decimal = Integer.parseInt(binario, 2);

        System.out.println("El número decimal equivalente es: " + decimal);
    }
}
```


