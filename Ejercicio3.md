# 🛠️ Ejercicio 3 (Java BigInteger)

¡En este problema tienes que sumar y multiplicar números enormes! Estos números son tan grandes que no puedes contenerlos en ningún tipo de datos ordinario, como un número entero largo.

## Descripción

Utilice el poder de la clase BigInteger de Java y resuelva este problema.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511544163529654334/image.png?ex=6a20d6b3&is=6a1f8533&hm=407a2b431a48f967cbe31f46c31d0b2a0aadef99cb666d866b85702f1a0c2226&" alt="DatosDeEntradaYSalida_Ejercicio3">
</div>

## Código Fuente

```
import java.io.*;
import java.util.*;
import java.math.BigInteger;

public class Solution {

    public static void main(String[] args) {
        //Julian Merino
        Scanner scanner = new Scanner(System.in);
        
        if (scanner.hasNextBigInteger()) {
            
            BigInteger a = scanner.nextBigInteger();
            BigInteger b = scanner.nextBigInteger();
            
            BigInteger sum = a.add(b);
            
            BigInteger product = a.multiply(b);
            
            System.out.println(sum);
            System.out.println(product);
        }
        
        scanner.close();
    }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511544323819442418/image.png?ex=6a20d6d9&is=6a1f8559&hm=800eb46235eba5774ce12c98d9f594430f3b6295cff3950f3115b70730bfca7f&" alt="ComprobacionEjercicio3">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
