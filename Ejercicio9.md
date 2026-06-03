# 🛠️ Ejercicio 9 (Java Method Overriding 2)

Cuando un método en una subclase anula un método en una superclase, aún es posible llamar al método anulado usando super palabra clave. Si escribes super.func() para llamar a la función func(), llamará al método que se definió en la superclase.

## Descripción

Se le proporciona un código parcialmente completo en el editor. Modifique el código para que imprima el siguiente texto:


```
Hello I am a motorcycle, I am a cycle with an engine.
My ancestor is a cycle who is a vehicle with pedals.
```
## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511565291426152458/image.png?ex=6a20ea61&is=6a1f98e1&hm=b97901354f04fc72b9d9c8b40e6877d2719497b4dee312e1165386d100d3ac8d&" alt="DatosDeEntradaYSalida_Ejercicio9">
</div>

## Código Fuente

```
import java.util.*;
import java.io.*;


class BiCycle{
	String define_me(){
		return "a vehicle with pedals.";
	}
}

class MotorCycle extends BiCycle{
	String define_me(){
		return "a cycle with an engine.";
	}
	
	MotorCycle(){
		System.out.println("Hello I am a motorcycle, I am "+ define_me());
        //Julian Merino
		String temp = super.define_me();

		System.out.println("My ancestor is a cycle who is "+ temp );
	}
	
}
class Solution{
	public static void main(String []args){
		MotorCycle M=new MotorCycle();
	}
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511565466894602341/image.png?ex=6a20ea8a&is=6a1f990a&hm=610f27e50027d751771b75911b07cd5c1f1c2e05d3eea51bd80958142057d837&" alt="ComprobacionEjercicio9">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
