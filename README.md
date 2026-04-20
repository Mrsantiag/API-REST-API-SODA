# Multidata Dashboard: Colombia y Rick y Morty

Este proyecto es una aplicacion web estatica que consume multiples APIs para visualizar informacion de interes publico y cultura pop en una sola interfaz limpia, minimalista y funcional.

## Documentacion de APIs Utilizadas

El sistema integra dos fuentes de datos externas mediante peticiones asincronas:

### 1. API Datos Abiertos Colombia (Socrata SODA)
* **Endpoint:** https://www.datos.gov.co/resource/hk5x-635y.json
* **Descripcion:** Proporciona el comparativo de clasificacion de planteles educativos en las Pruebas Saber 11 (ICFES).
* **Datos extraidos:** * Municipio de ubicacion.
    * Nombre de la Institucion Educativa.
    * Resultados categoricos (A+, A, B, C, D) desde el año 2014 hasta el 2024.
* **Funcionalidad:** Los datos se procesan localmente para generar filtros de busqueda dinamicos y un selector por municipio.

### 2. The Rick and Morty API
* **Endpoint:** https://rickandmortyapi.com/api/character/
* **Descripcion:** API de acceso abierto para obtener informacion sobre personajes de la serie.
* **Datos extraidos:** * Nombre del personaje.
    * Imagen oficial.
    * Estado (Vivo, Muerto o Desconocido).
    * Especie.
* **Funcionalidad:** Se realizan multiples consultas paralelas (Promise.all) para traer los primeros 20 personajes y visualizarlos en tarjetas de informacion.

## Caracteristicas Tecnicas

* Filtros Avanzados: Implementacion de logica de filtrado cruzado en JavaScript para el dataset de educacion.
* Diseno Clean and White: Interfaz enfocada en la legibilidad, sin animaciones ni efectos de movimiento, utilizando una paleta de colores profesional.
* Peticiones Asincronas: Uso de Fetch API y manejo de promesas para garantizar la carga de datos sin recargar la pagina.
* Disposicion Responsiva: Uso de CSS Grid y Flexbox para adaptar las tarjetas a cualquier tamano de pantalla.

## Estructura del Proyecto

---
├── index.html   # Logica unificada (HTML, CSS y JS)
└── README.md    # Documentacion tecnica del proyecto
---

## Instrucciones de Uso

1. Navegacion: Utiliza los botones superiores (Pruebas ICFES / Rick and Morty) para alternar entre las fuentes de datos.
2. Consulta ICFES: Filtra por nombre de colegio o selecciona un municipio especifico de Risaralda.
3. Consulta Rick and Morty: Visualiza la ficha tecnica de los personajes principales.

## Autores

* Santiago Perez
* Sebastian Lanco

---
Desarrollado con fines academicos para la exploracion de APIs y visualizacion de datos.
