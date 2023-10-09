<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


<!-- Actividad 08 -->
# Actividad: Ejecicios de métodos en Java
Implementar los siguientes métodos:


1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.
2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.
3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.
4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.
5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

## Solución
1.     

```java
package com.mycompany.actividad08;

import java.util.Scanner;

public class MayorDe_Dos {

    public static void main(String[] args) {
        int numero1 = 5;
        int numero2 = 8;

        int resultado = obtenerMayor(numero1, numero2);

        System.out.println("El mayor de los dos números es: " + resultado);
    }

    public static int obtenerMayor(int num1, int num2) {
        if (num1 > num2) {
            return num1;
        } else {
            return num2;
        }
    }
}

```





