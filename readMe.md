# 📚 Sistema de Planificación Modular Web — DETP / MINERD

Sistema automatizado de maquetación, visualización interactiva y exportación a PDF para planificaciones curriculares bajo el enfoque por competencias (Ordenanza 07-2025, DETP / MINERD), adaptado para centros técnicos como el Colegio APEC Fernando Arturo de Meriño (CAFAM).

---

## 📌 Descripción

Este repositorio contiene la arquitectura de interfaz web diseñada para transformar mallas curriculares y datos de ponderación oficial en documentos web interactivos y continuos.

El sistema resuelve la dispersión de documentos mediante un portal principal (`index.html`) que indexa los módulos formativos generados, cada uno dotado de navegación ancla multi-RA, preservación de colores institucionales y estilos de impresión optimizados (_pixel-perfect_) para la descarga directa en formato PDF tamaño Carta (Letter).

---

## 🚀 Características Principales

- **Portal Principal (`index.html`):** Tablero institucional con acceso directo a cada módulo formativo.
- **Navegación Superior Fija (_Sticky Toolbar_):** Acceso rápido mediante botones ancla a cada Resultado de Aprendizaje (`#raX-X`) y botón de impresión directa.
- **Estructura Modular Completa por RA:** Cada RA incluye encabezado oficial con logos, franja de actualización docente, tabla de datos generales y tabla de priorización/ponderación completa (39 semanas / 100%).
- **Tabla de Actividades de 6 Columnas:** Matriz pedagógica con Elemento de Capacidad (EC), Nivel de Dominio, Actividades con Evidencias en Taxonomía de Bloom (Niveles 3 y 4), Fechas, Instrumentos de Evaluación y Contenidos Mediadores.
- **Optimización de Impresión y PDF:** Configuración `@media print` con `-webkit-print-color-adjust: exact;`, márgenes seguros para evitar cortes del marco perimetral derecho y saltos de página limpios por cada RA (`page-break-before: always;`).

---

## 📂 Estructura del Repositorio

```text
├── index.html            # Portal principal con enlaces a los módulos
├── logoCafam.png         # Escudo oficial de la institución CAFAM
├── logoDETP.png          # Isotipo oficial de la DETP / Educación
├── INCO-MF032_3.html     # Módulo: Análisis y Diseño de Sistemas Informáticos
├── INCO-MF037_3.html     # Módulo: Análisis y Diseño de Reporte
├── INCO-MF038_3.html     # Módulo: Implementación y Mantenimiento de Aplicaciones
├── MF_464_3.html         # Módulo: Mantenimiento de Circuitos Microprogramables
└── MF_468_3.html         # Módulo: Mantenimiento de Sistemas Electrónicos de Potencia
```

---

## 🛠️ Tecnologías Empleadas

- **HTML5:** Estructura semántica continua y divisiones modulares.
- **CSS3:** Variables nativas para cromática institucional, maquetación flexible (_ Flexbox_ y _Grid_) y reglas avanzadas de impresión (`@page`, `@media print`).
- **JavaScript Nativo:** Ejecución de `window.print()` y anclaje con _scroll_ suave.

---

## 🎨 Paleta Cromática Institucional

| Código HEX | Uso / Sección                                      |
| :--------- | :------------------------------------------------- |
| `#A9D18E`  | Encabezados de RA y títulos principales            |
| `#C5E0B4`  | Cabecera de la tabla de actividades                |
| `#BDD7EE`  | Datos de bachillerato, códigos y campos técnicos   |
| `#FCE4D6`  | Cabecera de contraste de competencias (EC vs CE)   |
| `#FFFF00`  | Resaltador de notas y consideraciones curriculares |
| `#000000`  | Bordes de tablas continuos y nítidos (1px solid)   |

---

## 🖨️ Instrucciones para Descargar en PDF

1. Abre el archivo `.html` del módulo correspondiente en cualquier navegador moderno (Chrome, Edge o Firefox).
2. Haz clic en el botón superior **«Descargar / Guardar como PDF»** o presiona `Ctrl + P`.
3. En el cuadro de diálogo de impresión:
   - **Destino:** Guardar como PDF.
   - **Tamaño de papel:** Carta (Letter).
   - **Gráficos en segundo plano:** Marcar casilla (habilitado) para visualizar los colores de celda oficiales.
4. Presiona **Guardar**.

---

## 📄 Marco Legal y Créditos

- **Marco Curricular:** Ordenanza 07-2025, Dirección de Educación Técnico Profesional (DETP / MINERD), República Dominicana.
- **Institución:** Colegio APEC Fernando Arturo de Meriño (CAFAM) — Regional 15-03.
- **Docente Responsable:** José Luis Mañón Rosario.

```

```
