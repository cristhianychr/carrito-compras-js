# Carrito de Compras con JavaScript

Aplicación web de ejemplo que simula la compra de cursos en línea. Permite añadir cursos al carrito, aumentar la cantidad cuando se vuelve a seleccionar un curso, eliminar artículos y conservar el contenido del carrito en el navegador mediante `localStorage`.

El proyecto forma parte de los ejercicios prácticos del curso **JavaScript Moderno: Guía Definitiva Construye +10 Proyectos**.

## Demo

[Ver el proyecto en GitHub Pages](https://cristhianychr.github.io/carrito-compras-js/)

## Vista previa

![Vista previa del Carrito de Compras](./img/preview.png)

## Funcionalidades implementadas

- Catálogo estático con 12 cursos de ejemplo.
- Añadir un curso al carrito desde su tarjeta.
- Si se añade otra vez un curso que ya está en el carrito, se incrementa su cantidad en lugar de crear una fila duplicada.
- Visualización en el carrito de la imagen, el nombre, el precio y la cantidad de cada curso.
- Eliminación individual de un curso del carrito.
- Opción para vaciar el carrito.
- Guardado del contenido del carrito en `localStorage`.
- Recuperación del carrito guardado cuando se vuelve a cargar la página.
- Actualización dinámica de la tabla del carrito mediante JavaScript.

## Tecnologías y recursos

- **HTML5** para la estructura del catálogo y del carrito.
- **CSS** para los estilos personalizados.
- **Skeleton CSS** para la cuadrícula y los componentes de diseño.
- **Normalize.css** para normalizar los estilos entre navegadores.
- **JavaScript** para la lógica del carrito y la manipulación del DOM.
- **LocalStorage** para conservar el carrito en el navegador.
- **JSON** para serializar y recuperar los datos almacenados.
- **Git, GitHub y GitHub Pages** para el control de versiones y la publicación.

## Conceptos de JavaScript practicados

- Selección de elementos del DOM con `querySelector`.
- Manejo de eventos con `addEventListener` y delegación de eventos.
- Prevención del comportamiento predeterminado con `preventDefault()`.
- Lectura de información desde elementos HTML y atributos `data-id`.
- Creación de objetos a partir de los datos de cada curso.
- Uso de arreglos y métodos como `some()`, `map()`, `filter()` y `forEach()`.
- Operador spread (`...`) para crear un nuevo arreglo.
- Desestructuración de objetos.
- Creación e inserción de elementos con `createElement()` y `appendChild()`.
- Actualización y limpieza del contenido del DOM.
- Persistencia de datos con `localStorage`.
- Conversión entre objetos JavaScript y cadenas JSON con `JSON.stringify()` y `JSON.parse()`.

## Estructura del proyecto

```text
carrito-compras-js/
├── css/
│   ├── custom.css
│   ├── normalize.css
│   └── skeleton.css
├── img/
│   ├── preview.png
│   ├── cart.png
│   ├── curso1.jpg
│   ├── curso2.jpg
│   ├── curso3.jpg
│   ├── curso4.jpg
│   ├── curso5.jpg
│   └── otros recursos gráficos
├── js/
│   └── app.js
├── index.html
├── .gitignore
└── README.md
```

## Ejecutar localmente

No se requiere instalar dependencias para ejecutar el proyecto.

1. Clona el repositorio:

   ```bash
   git clone https://github.com/cristhianychr/carrito-compras-js.git
   ```

2. Accede a la carpeta:

   ```bash
   cd carrito-compras-js
   ```

3. Abre `index.html` en el navegador. También puedes abrir el proyecto con Visual Studio Code y utilizar una extensión como Live Server.

## Alcance y consideraciones

- Los cursos y precios están escritos directamente en el HTML; no proceden de una API ni de una base de datos.
- El carrito se guarda únicamente en el almacenamiento local del navegador. No se sincroniza entre dispositivos ni usuarios.
- El proyecto no procesa pagos ni completa compras reales.
- La página incluye un campo de búsqueda visual, pero en el JavaScript actual no se implementa una función de búsqueda.
- La acción **Vaciar carrito** utiliza `localStorage.clear()`, que borra todas las claves del almacenamiento local del mismo origen, no solamente la clave `carrito`.

## Curso

Proyecto desarrollado como ejercicio de aprendizaje del curso **JavaScript Moderno: Guía Definitiva Construye +10 Proyectos**.

## Autor

**Cristhian Chanamé**  
Estudiante de Ingeniería de Software.
