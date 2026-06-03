# 🛠️ Ejercicio 4 (Java Inheritance I)

Usando herencia, una clase puede adquirir las propiedades de otras. 

## Descripción

Considere lo siguiente Animal clase:
```
clase Animal{
    void caminar(){
        Sistema.fuera.println("Estoy caminando");
    }
}
```

Esta clase tiene un solo método, caminar. A continuación, queremos crear un Pá pájaro clase que también tiene una volar método. Hacemos esto usando extiende palabra clave:

```
clase Pá pájaro extiende Animal {
    void volar() {
        Sistema.fuera.println("Estoy volando");
    }
}
```

Finalmente, podemos crear un objeto Bird que pueda ambos volar y caminar.

```
público clase Solución{
   público estático void principal(Cadena[] args){

      Pá pájaro pájaro = nuevo Pá pájaro();
      pájaro.caminar();
      pájaro.volar();
   }
}
```
## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511547850633384126/image.png?ex=6a20da22&is=6a1f88a2&hm=8dbad43891f7e9716dd32b8ad1edcd230a9b4744e0567595042d81cbb57242c6&" alt="DatosDeEntradaYSalida_Ejercicio4">
</div>

## Código Fuente

```
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

class Animal{
	void walk()
	{
		System.out.println("I am walking");
	}
}
class Bird extends Animal
{
	void fly()
	{
		System.out.println("I am flying");
	}
    //Julian Merino
    void sing()
    {
        System.out.println("I am singing");
    }
}

public class Solution{

   public static void main(String args[]){

	  Bird bird = new Bird();
	  bird.walk();
	  bird.fly();
      bird.sing();
	
   }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511548080208740382/image.png?ex=6a20da59&is=6a1f88d9&hm=52d4e9e178a14f03677dd5ff9653a3c75a5636bef6e3e8040b24b33945549ca7&" alt="ComprobacionEjercicio4">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
