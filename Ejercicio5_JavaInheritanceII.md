# 🛠️ Ejercicio 5 (Java Inheritance II)

Escribe el siguiente código en tu editor a continuación:

## Descripción

1. Una clase llamada Aritmética con un método llamado agregar eso toma números enteros como parámetros y devuelve un número entero que indica su suma.

2. Una clase llamada Sumador que hereda de una superclase llamada Aritmética.


Tus clases no deberían serlo $public$.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511549249555271781/image.png?ex=6a20db70&is=6a1f89f0&hm=34a57cbbed71ae8041bb84c1e9dfdbf923e041661cebb7cb63b7e415e3a4db7f&" alt="DatosDeEntradaYSalida_Ejercicio5">
</div>

## Código Fuente

```
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;
//Julian Merino
class Arithmetic {
    int add(int a, int b) {
        return a + b;
    }
}

class Adder extends Arithmetic {
    
}

public class Solution{
    public static void main(String []args){
        // Create a new Adder object
        Adder a = new Adder();
        
        // Print the name of the superclass on a new line
        System.out.println("My superclass is: " + a.getClass().getSuperclass().getName());	
        
        // Print the result of 3 calls to Adder's `add(int,int)` method as 3 space-separated integers:
        System.out.print(a.add(10,32) + " " + a.add(10,3) + " " + a.add(10,10) + "\n");
     }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511549406917296299/image.png?ex=6a20db95&is=6a1f8a15&hm=52f4a2258ed9adec06d1e281c051b3a834166f00450441681f9b26c48d746d03&" alt="ComprobacionEjercicio5">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
