# 🛠️ Ejercicio 8 (Java method Overriding)

Cuando una subclase hereda de una superclase, también hereda sus métodos; sin embargo, también puede anular los métodos de superclase (así como declarar e implementar otros nuevos). 

## Descripción

Considere lo siguiente Deportes clasa:

```
clase Deportes{
    Cadena obtener nombre(){
        retorno „Deporte generic";
    }
    void obtenerNúmeroDeMiembrosDelEquipo(){
        Sistema.fuera.imprimir( "Cada equipo tiene n jugadores en " + obtener nombre() );
    }
}
```

A continuación, creamos un Fútbol clase que hereda de la Deportes clase. Podemos anular el obtener nombre método y devuelve una cadena diferente y específica de subclase:

```
clase Fútbol extiende Deportes{
    @Override
    Cadena obtener nombre(){
        retorno "Clase de fútbol";
    }
}
```

Nota: Al anular un método, debe precederlo con el @Override anotación. El parámetro(s) y el tipo de retorno de un método anulado deben ser exactamente los mismos que los del método heredado del supertipo.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511556578854174820/image.png?ex=6a20e243&is=6a1f90c3&hm=a0b25254467937452177eec1c4d80ff55e259022a1d968b4cffa67a9ca33e020&" alt="DatosDeEntradaYSalida_Ejercicio8">
</div>

## Código Fuente

```
import java.util.*;
class Sports{

    String getName(){
        return "Generic Sports";
    }
  
    void getNumberOfTeamMembers(){
        System.out.println( "Each team has n players in " + getName() );
    }
}

class Soccer extends Sports{
    @Override
    String getName(){
        return "Soccer Class";
    }
//Julian Merino
    @Override
    void getNumberOfTeamMembers() {
        System.out.println("Each team has 11 players in " + getName());
    }

}

public class Solution{
	
    public static void main(String []args){
        Sports c1 = new Sports();
        Soccer c2 = new Soccer();
        System.out.println(c1.getName());
        c1.getNumberOfTeamMembers();
        System.out.println(c2.getName());
        c2.getNumberOfTeamMembers();
	}
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511558925860995072/image.png?ex=6a20e473&is=6a1f92f3&hm=1ae765fe9bcfd3e7e618c8c353c173aad0209c94868686c2d58c21f1660d60b6&" alt="ComprobacionEjercicio8">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
