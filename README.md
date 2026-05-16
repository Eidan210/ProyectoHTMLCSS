# CostEstimater 📈

**CostEstimater** (también referenciado como *CostoDev App*) es una aplicación web interactiva y responsiva diseñada por Eidan Cuadros,  para que emprendedores, empresas y desarrolladores puedan estimar de forma instantánea, precisa y transparente el costo de sus proyectos de software mediante flujos interactivos.

La plataforma guía al usuario a través de un ecosistema visual por pasos (cuestionario de requerimientos, desglose financiero por fases y sección de contacto/recursos) para ofrecer presupuestos simulados detallados que ayudan a impulsar el desarrollo digital.

---

## 🚀 Características Principales

* **Precisión Inigualable:** Uso de interfaces intuitivas preparadas para algoritmos simulados de cálculo exacto de horas y costos de desarrollo.
* **Resultados Rápidos:** Obtención de una estimación completa y detallada del presupuesto en cuestión de minutos.
* **Transparencia Total:** Desglose financiero por etapas (Diseño, Frontend, Backend, Pruebas) eliminando costos ocultos.
* **Interfaz Moderna y Adaptativa:** Diseño completamente responsivo (adaptado a dispositivos móviles y escritorio) con transiciones dinámicas de carga (`fadeUp`), barras de progreso interactivas y componentes de selección amigables.

---

## 📂 Estructura del Proyecto

El proyecto está construido utilizando tecnologías web estándar de Front-End (**HTML5** y **CSS3**) y está organizado de la siguiente manera:

```bash
├── login.html          # Vista de aterrizaje (Landing Page) / Bienvenida general al estimador
├── login.css           # Estilos de inicio, configuración de variables globales (:root) y layout base
├── cuestionario.html   # Paso 1: Formulario interactivo de selección de plataforma (Web, Android, iOS)
├── cuestionario.css    # Estilos del formulario, contenedor de progreso y tarjetas de opción (cards)
├── Costos.html         # Pasos 2 y 3: Desglose simulado de costos de desarrollo y tabla detallada de fases
├── Costos.css          # Estilos de las barras porcentuales por fase y tablas de datos adaptativas
├── Resumen.html        # Paso 4: Formulario de contacto final, resumen de solicitud y recursos educativos
└── Resumen.css         # Estilos de la interfaz de cierre, cuadrículas de recursos y pie de página