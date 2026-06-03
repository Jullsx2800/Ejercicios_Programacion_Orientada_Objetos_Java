# 🛠️ Ejercicio 1 (Java BigDecimal)

La clase BigDecimal de Java puede manejar números decimales con signo de precisión arbitraria. 

## Descripción

Dada una matriz, $s$ , $n$ de cadenas de números reales, ordenelas en orden descendente — pero espera, ¡hay más! Cada número debe imprimirse exactamente en el mismo formato en el que fue leído desde stdin, lo que significa que $.1$ se imprime como $.1$, y $0.1$ se imprime como . Si dos números representan valores numéricamente equivalentes (por ejemplo, $.1 = 0.1$), entonces deben enumerarse en el mismo orden en que se recibieron como entrada).

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511539186115547308/image.png?ex=6a20d211&is=6a1f8091&hm=bea135f067cf962f6d1bb7b250c815d5bd535aaabd6a5666cc19bad16ddd14c0&" alt="DatosDeEntradaYSalida_Ejercicio1">
</div>

## Código Fuente

```
import java.math.BigDecimal;
import java.util.*;
class Solution{
    public static void main(String []args){
        //Input
        Scanner sc= new Scanner(System.in);
        int n=sc.nextInt();
        String []s=new String[n+2];
        for(int i=0;i<n;i++){
            s[i]=sc.next();
        }
        sc.close();

//Julian Merino        
        Arrays.sort(s, 0, n, (String s1, String s2) -> {

            BigDecimal b1 = new BigDecimal(s1);
            BigDecimal b2 = new BigDecimal(s2);
            
            return b2.compareTo(b1);
        });

        //Output
        for(int i=0;i<n;i++)
        {
            System.out.println(s[i]);
        }
    }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511539980051419346/image.png?ex=6a20d2ce&is=6a1f814e&hm=fb1bdfe835a2004cdbeeddad9cd07038c6a420e2558d51168811680a83708f00&" alt="ComprobacionEjercicio1">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
