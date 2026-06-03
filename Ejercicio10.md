# 🛠️ Ejercicio 10 (Java Instance of KeyWord)

El Java instancia de El operador se utiliza para probar si el objeto o instancia es una instancia del tipo especificado.

En este problema te hemos dado tres clases en el editor:

- Clase de estudiantes
- Clase estrella de rock
- Clase de hacker

En el método principal, completamos un Lista de matrices con varias instancias de estas clases. contar El método calcula cuántas instancias de cada tipo están presentes en ArrayList. El código imprime tres números enteros: el número de instancias de la clase Student, el número de instancias de la clase Rockstar y el número de instancias de la clase Hacker.

## Descripción

Pero faltan algunas líneas del código y hay que solucionarlo modificando únicamente $3$ ¡líneas! No agregue, elimine ni modifique ninguna línea adicional.

Para restaurar el código original en el editor, haga clic en el ícono superior izquierdo del editor y cree un nuevo búfer.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511566548983353493/image.png?ex=6a20eb8c&is=6a1f9a0c&hm=dea47e1b305226c3aa2423b26e4471a5fb2ef20dd9ef49cb58ad812bc74c3a47&" alt="DatosDeEntradaYSalida_Ejercicio10">
</div>

## Código Fuente

```
import java.util.*;

class Student{}
class Rockstar{   }
class Hacker{}


public class InstanceOFTutorial{
	
   static String count(ArrayList mylist){
      int a = 0,b = 0,c = 0;
      for(int i = 0; i < mylist.size(); i++){
         Object element=mylist.get(i);
         if(element instanceof Student)
            a++;
         if(element instanceof Rockstar)
            b++;
         if(element instanceof Hacker)
            c++;
      }
      String ret = Integer.toString(a)+" "+ Integer.toString(b)+" "+ Integer.toString(c);
      return ret;
   }

   public static void main(String []args){
      ArrayList mylist = new ArrayList();
      Scanner sc = new Scanner(System.in);
      int t = sc.nextInt();
      for(int i=0; i<t; i++){
         String s=sc.next();
         if(s.equals("Student"))mylist.add(new Student());
         if(s.equals("Rockstar"))mylist.add(new Rockstar());
         if(s.equals("Hacker"))mylist.add(new Hacker());
      }
      System.out.println(count(mylist));
   }
}


```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511566883877421086/image.png?ex=6a20ebdc&is=6a1f9a5c&hm=2e632410dc1bfbc7c9bfc841015eb6f91a1bbce548a9e3347fbee2405f746d1c&" alt="ComprobacionEjercicio10">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
