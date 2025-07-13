# 🧠 Mapa Mental desde CSV (con D3.js)

Este proyecto es una **aplicación web offline** que genera un grafo tipo árbol (tidy tree) a partir de un archivo **CSV local**, utilizando la biblioteca [D3.js](https://d3js.org/).

Cada fila del CSV representa una jerarquía de conceptos ejemplo como:

Vendedor → Fecha de Status → Cliente → [País, Tipo de Proyecto, Estado, Responsable, Status]


## 🚀 ¿Cómo usar?

1. Cloná o descargá este repositorio.
2. Abrí el archivo `index.html` directamente en tu navegador (doble clic).
3. Subí un archivo `.csv` con las siguientes columnas:

Vendedor,Fecha de Status,Cliente,País,Tipo de Proyecto,Estado,Responsable,Status


4. Al hacer clic en los nodos del grafo, podés colapsar y expandir jerarquías.

## 📌 Requisitos del CSV

- El archivo debe tener una fila de cabecera (headers).
- El orden y nombre de las columnas debe coincidir exactamente (inclusive mayúsculas y minúsculas).
- Ejemplo de fila:

Juan Perez,2024-05-10,Empresa Z,Argentina,Consultoría,Activo,Lucía Gómez,En revisión


## ✅ Características

- Visualización jerárquica interactiva con zoom y pan.
- Nodos colapsables / expandibles al hacer clic.
- Funciona completamente **sin conexión a Internet**.
- Compatible con navegadores modernos (Brave, Chrome, Firefox).
- Usa `d3.v7.min.js` descargado localmente para soporte offline.

## 📂 Estructura del proyecto

/tu-proyecto/
│
├── index.html ← Aplicación principal
├── d3.v7.min.js ← Librería D3.js (versión 7, version url online, aunque puede hacerse local también)
└── README.md ← Este archivo


## 💡 ¿Por qué usar D3.js?

D3.js es una biblioteca poderosa para crear visualizaciones de datos dinámicas e interactivas. En este proyecto, usamos:

- `d3.tree()` para organizar el grafo.
- `d3.hierarchy()` para estructurar los datos.
- `d3.zoom()` para navegación fluida.
- Soporte para CSV local con `d3.csvParse()`.

## 🛡️ Licencia

Este proyecto es de uso libre y educativo. Podés adaptarlo o extenderlo como desees.

---

**Desarrollado con ❤️ por Marce + D3.js**
