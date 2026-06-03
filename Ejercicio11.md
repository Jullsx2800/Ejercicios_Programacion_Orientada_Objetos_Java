# 🛠️ Ejercicio 11 (Java Iterator)

La clase Java Iterator puede ayudarle a iterar a través de cada elemento de una colección. 

## Descripción

He aquí un ejemplo sencillo:

```

importar java.util.*;
público clase Ejemplo{

    público estático void principal(Cadena []args){
        Lista de matrices mylist = nuevo Lista de matrices();
        mylist.agregar("Hola");
        mylist.agregar(„Java");
        mylist.agregar("4");
        Iterador it = mylist.iterador();
        mientras(it.tieneSiguiente()){
            Objeto elemento = it.siguiente();
            Sistema.fuera.println((Cadena)elemento);
        }
    }
}

```

En este problema necesitas completar un método func. El método requiere un Lista de matrices como entrada. En eso Lista de matrices hay uno o más números enteros, luego hay una cadena especial "###", después hay una o más cadenas diferentes. Una muestra Lista de matrices podría verse así:

```
element[0]=>42
element[1]=>10
element[2]=>"###"
element[3]=>"Hello"
element[4]=>"Java"
```
## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511569208624943114/image.png?ex=6a20ee06&is=6a1f9c86&hm=b9e31340a4610142126ba8a546f9afe6b67b8089fe8ec551a57def80414bb6a0&" alt="DatosDeEntradaYSalida_Ejercicio11">
</div>

## Código Fuente

```
import java.util.*;
public class Main{
	
   static Iterator func(ArrayList mylist){
      Iterator it=mylist.iterator();
      while(it.hasNext()){
         //Julian Merino
         Object element = it.next();
         if(element instanceof String)

			break;
		}
      return it;
      
   }
   @SuppressWarnings({ "unchecked" })
   public static void main(String []args){
      ArrayList mylist = new ArrayList();
      Scanner sc = new Scanner(System.in);
      int n = sc.nextInt();
      int m = sc.nextInt();
      for(int i = 0;i<n;i++){
         mylist.add(sc.nextInt());
      }
      
      mylist.add("###");
      for(int i=0;i<m;i++){
         mylist.add(sc.next());
      }
      
      Iterator it=func(mylist);
      while(it.hasNext()){
         Object element = it.next();
         System.out.println((String)element);
      }
   }
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511571904467832983/image.png?ex=6a20f089&is=6a1f9f09&hm=903472c522e361b6e870c06cbbf003733cf1c6aaf41508f40abee97db76eb018&" alt="ComprobacionEjercicio11">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
