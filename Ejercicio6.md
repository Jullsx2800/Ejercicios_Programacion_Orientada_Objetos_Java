# 🛠️ Ejercicio 6 (Java Abstract Class)

Una clase abstracta de Java es una clase que no se puede instanciar. Esto significa que no puedes crear nuevas instancias de una clase abstracta. Funciona como base para subclases. Deberías aprender sobre la herencia de Java antes de intentar este desafío.

## Descripción

A continuación se muestra un ejemplo de clase abstracta:

```
abstracto clase Libro{
    Cadena título;
    abstracto void establecer título(Cadena s);
    Cadena obtener título(){
        retorno título;
    }
}
```

Si intenta crear una instancia de esta clase como la siguiente línea, obtendrá un error:

```
Libro nueva_novela=nuevo Libro(); 
```
Tienes que crear otra clase que extienda la clase abstracta. Luego puedes crear una instancia de la nueva clase.

Tenga en cuenta que establecer título el método también es abstracto y no tiene cuerpo. Eso significa que debes implementar el cuerpo de ese método en la clase infantil.

En el editor hemos proporcionado el resumen Libro clase y a Principal clase. En la clase principal, creamos una instancia de una clase llamada Mi libro. Tu tarea es escribir solo el Mi libro clase.

Tu clase no debe ser pública.

## Datos de Entrada y Salida

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511551530430369835/image.png?ex=6a20dd90&is=6a1f8c10&hm=ef2ccba7f256c2eb139b0c009e102441f674cf117fd09489c316ee3343300180&" alt="DatosDeEntradaYSalida_Ejercicio6">
</div>

## Código Fuente

```
import java.util.*;
abstract class Book{
	String title;
	abstract void setTitle(String s);
	String getTitle(){
		return title;
	}
	
}
//Julian Merino
class MyBook extends Book {
    
    void setTitle(String s) {
        title = s;
    }
    
}

public class Main{
	
	public static void main(String []args){
		//Book new_novel=new Book(); This line prHMain.java:25: error: Book is abstract; cannot be instantiated
		Scanner sc=new Scanner(System.in);
		String title=sc.nextLine();
		MyBook new_novel=new MyBook();
		new_novel.setTitle(title);
		System.out.println("The title is: "+new_novel.getTitle());
      	sc.close();
		
	}
}

```
## Comprobación por HackerRank

<div align="center">
  <img src="https://cdn.discordapp.com/attachments/1494512379105509467/1511551854730022993/image.png?ex=6a20dddd&is=6a1f8c5d&hm=bf8c2a8d73fcc2fcbc6e9e4150cf26bf4d8117a0abf8e6b87109238c0dbe2125&" alt="ComprobacionEjercicio6">
</div>

<p align="right">
  <a href="Index.md">Volver a la página principal</a>
</p>
