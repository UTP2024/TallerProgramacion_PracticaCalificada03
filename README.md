
# Proyecto de Gestión de Autores y Publicaciones

![Diagrama de Clases](diagramaclases.png)

Este proyecto tiene como objetivo gestionar autores y sus publicaciones mediante clases y métodos definidos en Java. A continuación, se describen las clases `Autor` y `Publicacion`, así como sus respectivos métodos y las interacciones entre ellas.

## Clase `Autor`

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

## Clase `Publicacion`

### Métodos
- `toString`: Retorna todos los atributos de la publicación.

## Controlador `ControladorAutor`

### Métodos
- `AgregarPublicacion`: Llama al método `AgregarPublicacion` de la clase `Autor` y propaga cualquier error a la vista.
- `ImprimirAutor`: Utiliza el método `toString` del `Autor` para imprimir los detalles del mismo.

## Vista `VistaAutor`

### Funcionalidades
- Crear dos autores, cada uno con tres publicaciones.
- Imprimir los autores con sus respectivas publicaciones utilizando los métodos definidos en las otras clases.

## `main`

No se requiere un menú para esta implementación; el código puede escribirse directamente en el método `main`. Uno de los autores a crear debe ser usted mismo, utilizando sus datos personales.
