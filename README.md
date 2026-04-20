# Multidata Dashboard: Colombia y Rick y Morty

Este proyecto es una aplicacion web estatica que consume multiples APIs para visualizar informacion de interes publico y cultura pop en una sola interfaz limpia, minimalista y funcional.

## Caracteristicas

* Doble Integracion de API:
    * Educacion: Consulta del historico de clasificacion de planteles (ICFES Saber 11) de la Gobernacion de Risaralda via datos.gov.co.
    * Entretenimiento: Visualizacion de personajes del multiverso a traves de la Rick and Morty API.
* Filtros Avanzados: Buscador por nombre de institucion y selector dinamico por municipio para los datos educativos.
* Diseno Clean and White: Interfaz enfocada en la legibilidad, sin animaciones ni efectos de movimiento, utilizando una paleta de colores profesional.
* Totalmente Responsivo: Adaptado para una visualizacion optima en dispositivos moviles, tablets y computadoras de escritorio.

## Tecnologias Utilizadas

* HTML5: Estructura semantica.
* CSS3: Diseno Grid, Flexbox y variables nativas para la gestion de colores.
* JavaScript Vanilla: Gestion de peticiones asincronas (Fetch API), manipulacion del DOM y logica de filtrado.
* Socrata SODA API: Para el acceso a datos abiertos del gobierno colombiano.

## Estructura del Proyecto

---
├── index.html   # Archivo principal unificado (HTML, CSS y JS)
└── README.md    # Documentacion del proyecto
---

## Despliegue

La pagina esta desplegada a traves de GitHub Pages. Puedes acceder al sitio mediante el enlace generado en la seccion de Settings de este repositorio.

## Instrucciones de Uso

1. Navegacion: Utiliza los botones superiores (Pruebas ICFES / Rick and Morty) para alternar entre las bases de datos.
2. Busqueda: En la seccion ICFES, escribe el nombre de un colegio o municipio para filtrar los resultados en tiempo real.
3. Selector: Usa el menu desplegable para aislar datos de un municipio especifico en Risaralda.

## Autores

* Santiago Perez
* Sebastian Lanco

---
Desarrollado con fines academicos para la exploracion de APIs y visualizacion de datos.
