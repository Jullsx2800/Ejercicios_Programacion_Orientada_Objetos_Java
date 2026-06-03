# 🛠️ Ejercicio 2 (Java Primality Test)

Un número primo es un número natural mayor que $1$ cuyos únicos divisores positivos son $1$ y él mismo. Por ejemplo, los primeros seis números primos son $2$, $3$, $5$, $7$, $11$, y $13$.

## Descripción

Dado un número entero grande, , utilice Java BigInteger clase' esProbablePrime método para determinar e imprimir si lo es prime o not prime.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511542506897149972/image.png?ex=6a20d528&is=6a1f83a8&hm=a4ff5971739ce0e979b3d0ed4844a540ece6f4b2ce1e084338f398284829f3eb&" alt="DatosDeEntradaYSalida_Ejercicio2">
</div>

## Código Fuente

```
import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.function.*;
import java.util.regex.*;
import java.util.stream.*;
import static java.util.stream.Collectors.joining;
import static java.util.stream.Collectors.toList;



public class Solution {
    public static void main(String[] args) throws IOException {
        //Julian Merino
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(System.in));

        String n = bufferedReader.readLine();
        
        BigInteger bigInt = new BigInteger(n);
        
        if (bigInt.isProbablePrime(100)) {
            System.out.println("prime");
        } else {
            System.out.println("not prime");
        }

        bufferedReader.close();
    }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511542714183843962/image.png?ex=6a20d55a&is=6a1f83da&hm=549809ca8e6bc599c50e79cd91e9d30298a1d9960f4b7191e3f982b9b6c931cb&" alt="ComprobacionEjercicio2">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
