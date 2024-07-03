
# Practica Calificada 3

Usando el Modelo Vista Controlador desarrollar el siguiente sistema segun las especificaciones del diagrama de clases y la documentacion dada   

<img src="diagramaclases.png" alt="Diagrama de Clases" width="500"/>


## Pregunta 1: Crear la clase `Publicacion`

Crear la clase segun el diagrama de clases y segun las siguientes indicaciones:

`Metodo`
- `toString`: Este método retornará todos los atributos de la publicación.

## Pregunta 2: Crear la clase `Autor`

Crear la clase segun el diagrama de clases y segun las siguientes indicaciones:

### Atributos
- `TamañoArreglo`: Representa el número máximo de publicaciones que el arreglo puede contener.

### Métodos
- `setCantidadPublicaciones`: Valida que el valor asignado no exceda el tamaño del arreglo de publicaciones y propaga un error si es así.
- `AgregarPublicacion`: Valida que no se exceda el máximo de publicaciones permitido por el arreglo y propaga un error si se intenta superar este límite.
- `toString`: Retorna el nombre del autor junto con sus publicaciones en el siguiente formato:
  ```
  Autor: Carlos
  Publicaciones:
    publicacion1.toString()
    publicacion2.toString()
    publicacion3.toString()
  ```

### Constructor
- Inicializa `CantidadPublicaciones` en cero.

## Pregunta 3: Crear la clase `ControladorAutor`

### Métodos
- `AgregarPublicacion`: Llama al método `AgregarPublicacion` de la clase `Autor` y propaga cualquier error a la vista.
- `ImprimirAutor`: Utiliza el método `toString` del `Autor` para imprimir los detalles del mismo.

## Pregunta 4: Crear la clase `VistaAutor`

### Funcionalidades
- Crear dos autores, cada uno con tres publicaciones.
- Imprimir los autores con sus respectivas publicaciones utilizando los métodos definidos en las otras clases.

No se requiere un menú para esta implementación; el código puede escribirse directamente en el método `main`. Uno de los autores a crear debe ser usted mismo, utilizando sus datos personales.
