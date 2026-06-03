# 🛠️ Ejercicio 7 (Java Interface)

Una interfaz Java solo puede contener firmas de métodos y campos. La interfaz se puede utilizar para lograr polimorfismo. En este problema, practicarás tus conocimientos sobre interfaces.

## Descripción

Se le proporciona una interfaz Aritmética avanzada que contiene una firma de método int divisor_suma(int n). Necesitas escribir una clase llamada MyCalculator que implemente la interfaz.

suma divisora La función simplemente toma un número entero como entrada y devuelve la suma de todos sus divisores. Por ejemplo los divisores de 6 son 1, 2, 3 y 6, entonces divisor_suma Debería devolver 12. El valor de n será como máximo 1000.

Lea el código parcialmente completado en el editor y complételo. Solo necesitas escribir la clase MyCalculator. Tu clase no debería ser pública.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511552683297996910/image.png?ex=6a20dea2&is=6a1f8d22&hm=bb59a290d03f549c6ff2137acaea0a873cfc1ce0c772b0c935ec85c6840665aa&" alt="DatosDeEntradaYSalida_Ejercicio7">
</div>

## Código Fuente

```
import java.util.*;
interface AdvancedArithmetic{
  int divisor_sum(int n);
}
//Julian Merino
class MyCalculator implements AdvancedArithmetic {
    
    public int divisor_sum(int n) {
        int sum = 0;
        for (int i = 1; i <= n; i++) {
            if (n % i == 0) {
                sum += i;
            }
        }
        return sum;
    }
    
}

class Solution{
    public static void main(String []args){
        MyCalculator my_calculator = new MyCalculator();
        System.out.print("I implemented: ");
        ImplementedInterfaceNames(my_calculator);
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.print(my_calculator.divisor_sum(n) + "\n");
      	sc.close();
    }
    /*
     *  ImplementedInterfaceNames method takes an object and prints the name of the interfaces it implemented
     */
    static void ImplementedInterfaceNames(Object o){
        Class[] theInterfaces = o.getClass().getInterfaces();
        for (int i = 0; i < theInterfaces.length; i++){
            String interfaceName = theInterfaces[i].getName();
            System.out.println(interfaceName);
        }
    }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511552850084368566/image.png?ex=6a20deca&is=6a1f8d4a&hm=973b5bf24bbe72e0cc619f969b2c1aa00ab41b53bb447efdafde1cff782c4d4e&" alt="ComprobacionEjercicio7">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
