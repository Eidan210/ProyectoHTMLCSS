# CostEstimater — estimador de costos de software (HTML y CSS)

Sitio web de 4 pantallas, hecho solo con **HTML5** y **CSS3**, que presenta un estimador de costos para proyectos de software. Recorre la bienvenida, un cuestionario de plataforma, el desglose de costos por fase y un formulario de contacto. Es un ejercicio de maquetación: los costos son de ejemplo y no hay lógica de cálculo.

Este repositorio es la **versión de desarrollo**, construida con una rama y un pull request por pantalla. La variante entregada como examen está en [`Examenhtml`](https://github.com/Eidan210/Examenhtml).

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-responsive_·_animaciones-1572B6?style=flat-square&logo=css&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font_Awesome-iconos-528DD7?style=flat-square&logo=fontawesome&logoColor=white)
![Git](https://img.shields.io/badge/Git-ramas_+_7_PRs-F05032?style=flat-square&logo=git&logoColor=white)
![Último commit](https://img.shields.io/github/last-commit/Eidan210/ProyectoHTMLCSS?style=flat-square&label=último%20commit)

![Pantalla de bienvenida de CostEstimater](docs/inicio.webp)

## El problema

Quien quiere encargar un software no sabe cuánto puede costar ni en qué se va el presupuesto. El reto era maquetar, solo con HTML y CSS, un flujo claro que guíe al usuario paso a paso y muestre un presupuesto desglosado y comprensible, adaptado a móvil y a escritorio.

## Tecnologías

| Tecnología | Para qué se usa |
| :--- | :--- |
| **HTML5** | 4 páginas enlazadas con un menú común: bienvenida, cuestionario, costos y contacto. |
| **CSS3** | Variables (`:root`), Flexbox y Grid, `@media` para responsive, `@keyframes` (`fadeUp`), `:hover` y selección de tarjetas con `:checked`. |
| **Font Awesome** | Iconografía del menú y las tarjetas. |
| **Git y GitHub** | Una rama por pantalla y 7 pull requests (6 fusionados), con commits descriptivos. |

## Funciones clave

- **Bienvenida** con propuesta de valor, llamada a la acción y tarjetas de beneficios.
- **Cuestionario de plataforma** (Web, Android, iOS) con tarjetas seleccionables marcadas solo con CSS, sin JavaScript.
- **Desglose de costos:** total estimado, barras de porcentaje por fase (diseño, frontend, backend y pruebas) y tabla de horas y precios.
- **Contacto:** formulario de solicitud, resumen y sección de recursos.
- **Responsive y animado:** se adapta a móvil y escritorio, con animaciones de entrada y efectos *hover*.

## Evidencias

| Cuestionario | Desglose de costos | Contacto |
| :---: | :---: | :---: |
| ![Cuestionario de plataforma](docs/cuestionario.webp) | ![Desglose de costos por fase](docs/costos.webp) | ![Formulario de contacto](docs/resumen.webp) |

### Flujo de trabajo con Git

Cada pantalla se desarrolló en su propia rama y se integró a `main` con un pull request:

```mermaid
gitGraph
    commit id: "estructura inicial"
    branch Login-html
    commit id: "login + animaciones"
    checkout main
    merge Login-html id: "PR #1"
    branch Cuestionario-html
    commit id: "cuestionario + hover"
    checkout main
    merge Cuestionario-html id: "PR #2"
    branch Costos-html
    commit id: "costos + tabla"
    checkout main
    merge Costos-html id: "PR #4"
    branch Resumen-html
    commit id: "paso 4: contacto"
    checkout main
    merge Resumen-html id: "PR #5"
    checkout Login-html
    commit id: "fix enlace del login"
    checkout main
    merge Login-html id: "PR #6"
    branch Readme-md
    commit id: "README"
    checkout main
    merge Readme-md id: "PR #7"
```

## Instalación y uso

Sin dependencias:

```bash
git clone https://github.com/Eidan210/ProyectoHTMLCSS.git
cd ProyectoHTMLCSS
```

Abre `login.html` en el navegador (o con **Live Server**) y avanza con **Comenzar**. Los iconos se cargan desde el kit de Font Awesome, así que necesitan conexión a internet.

```text
ProyectoHTMLCSS/
├── login.html · login.css                 # Bienvenida
├── cuestionario.html · cuestionario.css   # Paso 1: plataforma
├── Costos.html · Costos.css               # Pasos 2-3: desglose de costos
├── Resumen.html · Resumen.css             # Paso 4: contacto y recursos
└── *.png                                  # Ilustraciones e iconos
```

## Aprendizajes

- **Maquetar un flujo de varias páginas** con estructura semántica y una navegación coherente.
- **Resolver interacción solo con CSS:** tarjetas seleccionables con `:checked` y efectos con `:hover`, sin una línea de JavaScript.
- **Diseño responsive** con Flexbox, Grid y `@media`, y animaciones de entrada con `@keyframes`.
- **Trabajar con ramas y pull requests:** una funcionalidad por rama, integraciones revisables y commits que explican el cambio.

---

Desarrollado por **Eidan Alexander Carreño** ([@Eidan210](https://github.com/Eidan210)) · Campuslands.
