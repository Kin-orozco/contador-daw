# Proyecto Contador - 1º DAW

Este repositorio contiene la solución a la práctica de **Entornos de Desarrollo**. Se trata de un contador reactivo construido con **Vue 3** y **Vite**.

## 🛠️ Tecnologías utilizadas
* **Framework:** Vue 3 (Composition API).
* **Calidad de Código:** ESLint para análisis estático.
* **Control de Versiones:** Git y GitHub.

## 📈 Proceso de Desarrollo
* **Análisis con ESLint**: Se detectaron y eliminaron variables no utilizadas (`nombre`, `mensajeOculto`) para limpiar el código.
* **Refactorización**: Se renombraron las funciones a `aumentar()` y `disminuir()` para mejorar la semántica.
* **Lógica de negocio**: El contador tiene límites estrictos entre 0 y 10.

## 📊 Diagrama de Clases (UML)
```mermaid
classDiagram
    class Contador {
        +int count
        +aumentar() void
        +disminuir() void
    }

Actualizada documentación
