# 🛠️ Ejercicio 12 (Java Exception Handling)

El manejo de excepciones es el proceso de responder a la ocurrencia, durante el cálculo, de excepciones – condiciones anómalas o excepcionales que requieren un procesamiento especial – que a menudo cambian el flujo normal de ejecución del programa. 

## Descripción

Java tiene un mecanismo incorporado para manejar excepciones. Usando el intentar declaración: podemos probar un bloque de código para detectar errores. El atrapar El bloque contiene el código que dice qué hacer si ocurre una excepción.

Este problema pondrá a prueba tus conocimientos sobre el bloque try-catch.

Se te darán dos números enteros y Como entrada, tienes que calcular $x/y$. Si $x$ y $y$ no lo son $32$ números enteros con signo de bits o si $y$ es cero, se producirá una excepción y tendrás que informarlo. Lea el ejemplo de entrada/salida para saber qué informar en caso de excepciones.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511573165447315476/image.png?ex=6a20f1b6&is=6a1fa036&hm=1ad6fed2aeecc22da5996adf05fd06724e860ac4136eb57b83a2177cb2d2304b&" alt="DatosDeEntradaYSalida_Ejercicio12">
</div>

## Código Fuente

```
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        //Julian Merino
        Scanner scanner = new Scanner(System.in);
        
        try {
            // Read inputs
            int x = scanner.nextInt();
            int y = scanner.nextInt();
            
            // Try to divide and print the result
            System.out.println(x / y);
            
        } catch (InputMismatchException e) {
            // Triggers if input is a string, float, or too large
            System.out.println("java.util.InputMismatchException");
            
        } catch (ArithmeticException e) {
            // Triggers if y is 0
            System.out.println(e);
            
        }
        
        scanner.close();
    }
}


```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511573389972606986/image.png?ex=6a20f1eb&is=6a1fa06b&hm=3a29d7310c93f9e54b7bea62b586a024840121693fdc02d252c6cdf1f4a33624&" alt="ComprobacionEjercicio12">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
