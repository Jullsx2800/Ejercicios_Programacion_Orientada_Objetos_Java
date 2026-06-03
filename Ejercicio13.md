# 🛠️ Ejercicio 13 (Java esception Handling)

Es necesario calcular la potencia de un número implementando una calculadora. Crea una clase Mi calculadora que consta de un único método long power(int, int). Este método toma dos números enteros, $n$ y $p$ , como parámetros y hallazgos $n^p$. Si cualquiera de los dos $n$ o $p$ es negativo, entonces el método debe generar una excepción que diga "$n or p should not be negative$". Además, si ambos $n$ y $p$ son cero, entonces el método debe lanzar una excepción que diga "$n and p should not be zero$"

## Descripción

Por ejemplo, -4 y -5 daría como resultado $Java.lang.Exception$ $: n$ $or$ $p$ $should$ $not$ $be$ $negative$ .

Completa la función power en clase Mi calculadora y devolver el resultado apropiado después de la operación de energía o una excepción apropiada como se detalla anteriormente.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511574976321421404/image.png?ex=6a20f366&is=6a1fa1e6&hm=5ded84f2f820836ca22882a22fc08d5f0c2004f39eae3b7bbe89f86a8866192a&" alt="DatosDeEntradaYSalida_Ejercicio13">
</div>

## Código Fuente

```
import java.util.Scanner;
class MyCalculator {
    //Julian Merino
    long power(int n, int p) throws Exception {
        if (n == 0 && p == 0) {
            throw new Exception("n and p should not be zero.");
        } else if (n < 0 || p < 0) {
            throw new Exception("n or p should not be negative.");
        } else {
            return (long) Math.pow(n, p);
        }
    }
}

public class Solution {
    public static final MyCalculator my_calculator = new MyCalculator();
    public static final Scanner in = new Scanner(System.in);
    
    public static void main(String[] args) {
        while (in .hasNextInt()) {
            int n = in .nextInt();
            int p = in .nextInt();
            
            try {
                System.out.println(my_calculator.power(n, p));
            } catch (Exception e) {
                System.out.println(e);
            }
        }
    }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511575282178461797/image.png?ex=6a20f3ae&is=6a1fa22e&hm=34ff70593acc82e71476a03da90012590d3e79acae69f9107619e334574bf535&" alt="ComprobacionEjercicio13">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
