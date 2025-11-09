# Gestión de Datos de Países en Python: Filtros, Ordenamientos y Estadísticas

## 📋 Índice

1.  [Descripción del Proyecto](#-descripción-del-proyecto)
2.  [Funcionalidades](#-funcionalidades)
3.  [Instrucciones de Uso](#-instrucciones-de-uso)
4.  [Ejemplos de Entradas y Salidas](#ejemplos-de-entradas-y-salidas)
5.  [Integrantes del Grupo 13](#integrantes-del-grupo-13)

---

## 📄 Descripción del Proyecto

Aplicación de consola desarrollada en **Python 3.x** para la gestión de un dataset de información geográfica y demográfica de países.

Este proyecto fue desarrollado como **Trabajo Práctico Integrador (TPI)** para la asignatura Programación 1.
El objetivo principal fue demostrar el dominio de **estructuras de datos complejas** (**Lista de Diccionarios**), la **modularización** mediante funciones y la **persistencia de datos** utilizando archivos **CSV**.

---

## ✨ Funcionalidades

El sistema opera mediante un menú interactivo y ofrece las siguientes capacidades:

- **Carga y Persistencia:** Lee y guarda datos en el archivo `paises.csv` utilizando el módulo `csv`.
- **CRUD Básico:** Permite **Agregar** nuevos países y **Actualizar** la población/superficie de países existentes.
- **Búsqueda:** Búsqueda de países por nombre (coincidencia parcial e insensible a mayúsculas/acentos).
- **Filtrado Avanzado:** Permite filtrar por **Continente** o por **Rango** de Población/Superficie.
- **Ordenamiento:** Ordena la lista de países por **Nombre, Población o Superficie**, de forma ascendente o descendente.
- **Estadísticas:** Calcula el país con **mayor/menor población**, el **promedio** de población/superficie, y el **conteo** de países por continente.
- **Validación Robusta:** Incluye funciones de validación para asegurar que las entradas de población y superficie sean números positivos.

---

## 🚀 Instrucciones de Uso

### Requisitos

- **Python 3.6** o superior.
- El programa utiliza únicamente los módulos estándar de Python (`csv`, `unicodedata`).

### Pasos para la Ejecución

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/aldimhernandez/UTN-TUPaD-Programacion1-TPI-Grupo-13.git
    ```
2.  **Navegar al directorio del proyecto:**
    ```bash
    cd UTN-TUPaD-Programacion1-TPI-Grupo-13
    ```
3.  **Ejecutar el archivo principal:**
    ```bash
    python .\src\202509_P1_TPI_ESCALANTE_HERNANDEZ.py
    ```
4.  El programa iniciará el menú de opciones en la consola.

---

## 🗂️ Ejemplos de Entradas y Salidas

| Operación                              | Entrada del Usuario                                                                                                          | Salida Esperada                                                                                      |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| **Búsqueda (Opción 2)**                | `Seleccione una opción: 2` <br> `Ingrese el nombre a buscar: arg`                                                            | Muestra en pantalla el país **Argentina** (coincidencia parcial).                                    |
| **Filtrado por Continente (Opción 3)** | `Seleccione una opción: 3` <br> `Ingrese criterio (c/p/s): c` <br> `Ingrese continente: Asia`                                | Muestra solo los países donde el campo `continente` es "Asia".                                       |
| **Agregar País (Opción 6)**            | `Seleccione una opción: 6` <br> `Nombre: Atlantis` <br> `Población: 1000` <br> `Superficie: 5000` <br> `Continente: Oceanía` | `✅ País agregado exitosamente.` <br> El nuevo país se añade a la lista y se guarda en `paises.csv`. |
| **Validación de Error**                | `Seleccione una opción: 6` <br> `Población: -50`                                                                             | `⚠️ La población debe ser un número positivo.`                                                       |
| **Ordenamiento (Opción 4)**            | `Seleccione una opción: 4` <br> `Criterio (n/p/s): p` <br> `Sentido (a/d): d`                                                | La lista se muestra ordenada por **Población, de forma Descendente (mayor a menor)**.                |

---

## 👥 Integrantes del Grupo 13

| Integrante                  | Comisión   | Email                   |
| :-------------------------- | :--------- | :---------------------- |
| **Escalante, Juan Facundo** | Comisión 5 | facuescalante@gmail.com |
| **Hernández, María Aldana** | Comisión 6 | marialdanahz@gamil.com  |
