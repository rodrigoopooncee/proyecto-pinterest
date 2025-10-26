# Proyecto 1: Arquitectura Semántica - Clon de Pinterest

Este repositorio contiene la primera entrega de la práctica de Arquitectura de la Información para el curso Full Stack de ThePower.

El objetivo del proyecto es crear un fichero HTML que estructure una aplicación similar a Pinterest. Siguiendo las instrucciones, el enfoque no está en replicar la página al completo, sino en **definir su arquitectura semántica** a grandes rasgos.

## Metodología y Enfoque

Siguiendo la recomendación de "pensar en cajas", este proyecto se ha estructurado utilizando rigurosamente las etiquetas semánticas de HTML5 (`<header>`, `<nav>`, `<main>`, `<article>`, etc.).

Para ir más allá de los requisitos mínimos y demostrar una visión de producto completa, tomé una serie de **decisiones estratégicas de cosecha propia**. Se utilizaron herramientas de IA como un asistente de ejecución para acelerar la implementación de estas ideas y asegurar las mejores prácticas de código, pero la visión y las mejoras de valor añadido son un aporte humano.

## Decisiones Estratégicas y Mejoras Implementadas

Para que el proyecto no fuera solo un ejercicio, sino un producto viable y de nivel profesional, decidí implementar las siguientes mejoras clave:

### 1. Optimización de Rendimiento Web (Performance)

* **Carga diferida de imágenes:** Se implementó el atributo `loading="lazy"` en todas las imágenes de la galería. Esto optimiza drásticamente el tiempo de carga inicial de la página.
* **Formatos de Imagen Modernos:** Se utiliza la etiqueta `<picture>` para servir imágenes en formato **.webp** (más ligero) siempre que sea posible, con un fallback a `.jpg` para navegadores antiguos. Esto reduce el peso total de la página y mejora la velocidad de carga.

### 2. SEO Técnico y Marketing

* **Metaetiquetas Avanzadas:** Se ha implementado un `<head>` completo, incluyendo `description` y `keywords` para el SEO.
* **URL Canónica:** Se incluye la etiqueta `<link rel="canonical">` para prevenir problemas de contenido duplicado, una práctica estándar de SEO.
* **Open Graph (OG Tags):** Se han añadido metaetiquetas de Open Graph para asegurar que el enlace se muestre de forma atractiva y profesional al ser compartido en redes sociales como WhatsApp o Twitter.
* **Schema.org (JSON-LD):** Se ha integrado un script de Schema.org para proporcionar a Google un contexto estructurado de la página, mejorando el posicionamiento.

### 3. Accesibilidad (A11y)

* **Descripciones de Imágenes:** Todas las imágenes cuentan con un atributo `alt` descriptivo y detallado, un requisito esencial tanto para la accesibilidad (lectores de pantalla) como para el SEO.

## Estructura del Proyecto

* `pinterest.html`: El archivo principal que contiene toda la arquitectura semántica.
* `README.md`: Este mismo archivo.

## Cómo Utilizar este Proyecto

1.  Clonar el repositorio.
2.  Abrir `pinterest.html` en cualquier navegador web.
3.  Se recomienda usar las herramientas de desarrollador del navegador (F12) para inspeccionar la estructura semántica del DOM y analizar la pestaña "Network" para verificar la carga eficiente de las imágenes.