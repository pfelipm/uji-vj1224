# 🎮 VJ1224 · Ingeniería del Software (Grado en Diseño y Desarrollo de Videojuegos · UJI)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Online-22d3ee?style=for-the-badge&logo=github)](https://pfelipm.github.io/uji-vj1224/)
[![Google Sites](https://img.shields.io/badge/Google%20Sites-VJ1224-facc15?style=for-the-badge&logo=google)](https://sites.google.com/uji.es/vj1224-2026)
[![Licencia: CC BY-NC-SA 4.0](https://img.shields.io/badge/Licencia-CC%20BY--NC--SA%204.0-34d399?style=for-the-badge)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)

Repositorio público de **aplicaciones web interactivas de página única (SPA)** utilizadas como material docente de apoyo en las sesiones de teoría de la asignatura **VJ1224 · Ingeniería del Software** (3.er curso, 1.er semestre) del **Grado en Diseño y Desarrollo de Videojuegos** de la **Universitat Jaume I (UJI)** de Castellón.

- **Profesor responsable de teoría y autor de los materiales:** [Pablo Felip Monferrer](https://www.pablofelip.uji.es/) (Departamento de Lenguajes y Sistemas Informáticos · UJI)
- **Catálogo interactivo en GitHub Pages:** [https://pfelipm.github.io/uji-vj1224/](https://pfelipm.github.io/uji-vj1224/)
- **Web docente en Google Sites:** [https://sites.google.com/uji.es/vj1224-2026](https://sites.google.com/uji.es/vj1224-2026)
- **Editor web educativo UML (AS-UML):** [https://umlsimple.pablofelip.online](https://umlsimple.pablofelip.online)

---

## 🛠️ Herramientas gratuitas de modelado UML en la asignatura

Para los bloques de **Temas 4, 5 y 6 (DCU, DC y DA)** se utiliza como herramienta docente principal **[Arquitecto Simple UML (AS-UML)](https://umlsimple.pablofelip.online)**, un editor web educativo de código abierto desarrollado específicamente para la asignatura (soporte directo para DCU, DC y DA con *swimlanes*, persistencia local, copias de seguridad JSON y exportación PNG). Como herramientas gratuitas complementarias se recomiendan:

- **Editores visuales (*Drag & Drop*):** [draw.io / diagrams.net](https://app.diagrams.net/), [Apollon Editor (TUM)](https://apollon.ase.in.tum.de/) y [Gaphor](https://gaphor.org/).
- **Diagramas como código (*Diagrams as Code* para Notion y GitHub):** [Mermaid.js](https://mermaid.live/) (integrado nativamente en bloques `/code` de Notion) y [PlantUML](https://www.planttext.com/).

---

## 🤖 Asistentes de IA de la asignatura (Gems de Google Gemini)

El ecosistema docente de VJ1224 integra tres asistentes conversacionales personalizados (**Gems**) entrenados específicamente para acompañar al estudiantado en el diseño, gestión ágil y modelado de arquitectura de su videojuego:

1. 🔮 **[El Oráculo (Product Owner)](https://gemini.google.com/gem/1MNB-Wb78FOJpZrOTtComZjmg8nXRdU92?usp=sharing)** — Simulador de cliente para las dinámicas de entrevista de elicitación de requisitos, redacción de historias de usuario y priorización del *Product Backlog* (Tema 2).
2. 🧘‍♂️ **[GameDev-Scrum Sensei](https://gemini.google.com/gem/1gyutyBOh6RUnwjhyVlKhJEPRTvrN0yEB?usp=sharing)** — Mentor experto en producción ágil con Scrum, auditoría del *Product Backlog*, criterios de aceptación en formato *Gherkin*, regla INVEST y desarrollo con Unity (Tema 3).
3. 📐 **[El Arquitecto de Blueprints](https://gemini.google.com/gem/1P3nO8hRPQJNATorPn5XojUgbZ-nooX_Q?usp=sharing)** — Copiloto socrático experto en modelado UML y patrones de diseño para videojuegos: revisa diagramas de casos de uso (DCU), clases (DC) y actividades (DA) sin regalar la solución hecha (Temas 4, 5 y 6).

---

## 🏗️ Arquitectura técnica e integración continua (GitHub Pages + Google Sites)

Todas las píldoras interactivas de este repositorio siguen una arquitectura **100 % autocontenida** y de **doble propósito**:

1. **Navegación web autónoma (GitHub Pages):**
   - Portal principal ([`index.html`](index.html)) con buscador instantáneo, filtrado por temas y copiado rápido de URLs.
   - Cada SPA incorpora una barra superior de navegación secuencial (`← Anterior | Índice general | Siguiente →`) para recorrer el temario sin interrupciones.
2. **Inserción limpia a página completa por URL en Google Sites (`is-embedded`):**
   - Cada SPA detecta automáticamente en el `<head>` si se está ejecutando dentro de un `<iframe>` (`window.self !== window.top`).
   - Al insertarse en Google Sites mediante **Insertar → Por URL**, la clase `.is-embedded` oculta de inmediato la barra de navegación superior redundante (`.hide-in-embed`), cediendo el 100 % del lienzo al contenido didáctico.
3. **Estética y ergonomía de proyección en aula (*High-Contrast Retro-HUD*):**
   - Tipografía dual (`Press Start 2P` para marcadores HUD y `Rajdhani` de alto gramaje para lectura nítida desde las últimas filas del aula).
   - Revelación progresiva (*progressive disclosure*) controlada tanto por botones en flujo natural como por teclado (`Espacio`, `→`, `←`) para acompañar el ritmo de explicación docente.

---

## 📚 Catálogo de píldoras interactivas y URLs directas para Google Sites

### 🎓 Presentación de la asignatura (Día 0)

| # | Píldora interactiva (SPA) | Archivo local | URL directa (GitHub Pages / Google Sites) |
| :-: | :--- | :--- | :--- |
| **00** | **Guía docente interactiva (día 0 - presentación)** | [`auxiliar/Guía docente interactiva (día 0 - presentación).html`](auxiliar/Gu%C3%ADa%20docente%20interactiva%20%28d%C3%ADa%200%20-%20presentaci%C3%B3n%29.html) | `https://pfelipm.github.io/uji-vj1224/auxiliar/Gu%C3%ADa%20docente%20interactiva%20%28d%C3%ADa%200%20-%20presentaci%C3%B3n%29.html` |

---

### ⚙️ Tema 1. La ingeniería del software y los videojuegos

| # | Píldora interactiva (SPA) | Archivo local | URL directa (GitHub Pages / Google Sites) |
| :-: | :--- | :--- | :--- |
| **01** | **La ingeniería del software** | [`t1/01 La ingeniería del software.html`](t1/01%20La%20ingenier%C3%ADa%20del%20software.html) | `https://pfelipm.github.io/uji-vj1224/t1/01%20La%20ingenier%C3%ADa%20del%20software.html` |
| **02** | **La crisis del software** | [`t1/02 La crisis del software.html`](t1/02%20La%20crisis%20del%20software.html) | `https://pfelipm.github.io/uji-vj1224/t1/02%20La%20crisis%20del%20software.html` |
| **03** | **Las leyes no escritas del desarrollo del software** | [`t1/03 Las leyes no escritas del desarrollo del software.html`](t1/03%20Las%20leyes%20no%20escritas%20del%20desarrollo%20del%20software.html) | `https://pfelipm.github.io/uji-vj1224/t1/03%20Las%20leyes%20no%20escritas%20del%20desarrollo%20del%20software.html` |
| **04** | **Cascada vs. ágil (Scrum)** | [`t1/04 Cascada vs. ágil (Scrum).html`](t1/04%20Cascada%20vs.%20%C3%A1gil%20%28Scrum%29.html) | `https://pfelipm.github.io/uji-vj1224/t1/04%20Cascada%20vs.%20%C3%A1gil%20%28Scrum%29.html` |
| **05** | **UML: los planos del videojuego** | [`t1/05 UML - los planos del videojuego.html`](t1/05%20UML%20-%20los%20planos%20del%20videojuego.html) | `https://pfelipm.github.io/uji-vj1224/t1/05%20UML%20-%20los%20planos%20del%20videojuego.html` |
| **06** | **El ecosistema Scrum** | [`t1/06 El ecosistema Scrum.html`](t1/06%20El%20ecosistema%20Scrum.html) | `https://pfelipm.github.io/uji-vj1224/t1/06%20El%20ecosistema%20Scrum.html` |
| **07** | **Scrum con Notion** | [`t1/07 Scrum con Notion.html`](t1/07%20Scrum%20con%20Notion.html) | `https://pfelipm.github.io/uji-vj1224/t1/07%20Scrum%20con%20Notion.html` |

---

### 🃏 Tema 2. Historias de usuario y gestión ágil de requisitos

| # | Píldora interactiva (SPA) | Archivo local | URL directa (GitHub Pages / Google Sites) |
| :-: | :--- | :--- | :--- |
| **01** | **La cita filosófica** | [`t2/01 La cita filosófica.html`](t2/01%20La%20cita%20filos%C3%B3fica.html) | `https://pfelipm.github.io/uji-vj1224/t2/01%20La%20cita%20filos%C3%B3fica.html` |
| **02** | **La jerarquía del diseño** | [`t2/02 La jerarquía del diseño.html`](t2/02%20La%20jerarqu%C3%ADa%20del%20dise%C3%B1o.html) | `https://pfelipm.github.io/uji-vj1224/t2/02%20La%20jerarqu%C3%ADa%20del%20dise%C3%B1o.html` |
| **03** | **Historias de usuario** | [`t2/03 Historias de usuario.html`](t2/03%20Historias%20de%20usuario.html) | `https://pfelipm.github.io/uji-vj1224/t2/03%20Historias%20de%20usuario.html` |
| **04** | **Historia vs. tarea** | [`t2/04 Historia vs. tarea.html`](t2/04%20Historia%20vs.%20tarea.html) | `https://pfelipm.github.io/uji-vj1224/t2/04%20Historia%20vs.%20tarea.html` |
| **05** | **Épica vs. historia** | [`t2/05 Épica vs. historia.html`](t2/05%20%C3%89pica%20vs.%20historia.html) | `https://pfelipm.github.io/uji-vj1224/t2/05%20%C3%89pica%20vs.%20historia.html` |
| **06** | **El viaje de la idea** | [`t2/06 El viaje de la idea.html`](t2/06%20El%20viaje%20de%20la%20idea.html) | `https://pfelipm.github.io/uji-vj1224/t2/06%20El%20viaje%20de%20la%20idea.html` |
| **07** | **La forja de la misión** | [`t2/07 La forja de la misión.html`](t2/07%20La%20forja%20de%20la%20misi%C3%B3n.html) | `https://pfelipm.github.io/uji-vj1224/t2/07%20La%20forja%20de%20la%20misi%C3%B3n.html` |
| **08** | **El diálogo del héroe** | [`t2/08 El diálogo del héroe.html`](t2/08%20El%20di%C3%A1logo%20del%20h%C3%A9roe.html) | `https://pfelipm.github.io/uji-vj1224/t2/08%20El%20di%C3%A1logo%20del%20h%C3%A9roe.html` |
| **09** | **La receta de una buena historia - INVEST** | [`t2/09 La receta de una buena historia - INVEST.html`](t2/09%20La%20receta%20de%20una%20buena%20historia%20-%20INVEST.html) | `https://pfelipm.github.io/uji-vj1224/t2/09%20La%20receta%20de%20una%20buena%20historia%20-%20INVEST.html` |
| **10** | **Puntos de historia** | [`t2/10 Puntos de historia.html`](t2/10%20Puntos%20de%20historia.html) | `https://pfelipm.github.io/uji-vj1224/t2/10%20Puntos%20de%20historia.html` |
| **11** | **Planning poker** | [`t2/11 Planning poker.html`](t2/11%20Planning%20poker.html) | `https://pfelipm.github.io/uji-vj1224/t2/11%20Planning%20poker.html` |
| **12** | **Definition of done** | [`t2/12 Definition of done.html`](t2/12%20Definition%20of%20done.html) | `https://pfelipm.github.io/uji-vj1224/t2/12%20Definition%20of%20done.html` |
| **13** | **El tablero Kanban** | [`t2/13 El tablero Kanban.html`](t2/13%20El%20tablero%20Kanban.html) | `https://pfelipm.github.io/uji-vj1224/t2/13%20El%20tablero%20Kanban.html` |
| **14** | **Briefing de misión** | [`t2/14 Briefing de misión.html`](t2/14%20Briefing%20de%20misi%C3%B3n.html) | `https://pfelipm.github.io/uji-vj1224/t2/14%20Briefing%20de%20misi%C3%B3n.html` |
| **15** | **La jerarquía de Notion** | [`t2/15 La jerarquía de Notion.html`](t2/15%20La%20jerarqu%C3%ADa%20de%20Notion.html) | `https://pfelipm.github.io/uji-vj1224/t2/15%20La%20jerarqu%C3%ADa%20de%20Notion.html` |

---

### 🛡️ Tema 3. Gestión ágil de proyectos con Scrum

| # | Píldora interactiva (SPA) | Archivo local | URL directa (GitHub Pages / Google Sites) |
| :-: | :--- | :--- | :--- |
| **01** | **Lean, Agile y Scrum** | [`t3/01 Lean, Agile y Scrum.html`](t3/01%20Lean%2C%20Agile%20y%20Scrum.html) | `https://pfelipm.github.io/uji-vj1224/t3/01%20Lean%2C%20Agile%20y%20Scrum.html` |
| **02** | **El origen de Scrum** | [`t3/02 El origen de Scrum.html`](t3/02%20El%20origen%20de%20Scrum.html) | `https://pfelipm.github.io/uji-vj1224/t3/02%20El%20origen%20de%20Scrum.html` |
| **03** | **El corazón de Scrum** | [`t3/03 El corazón de Scrum.html`](t3/03%20El%20coraz%C3%B3n%20de%20Scrum.html) | `https://pfelipm.github.io/uji-vj1224/t3/03%20El%20coraz%C3%B3n%20de%20Scrum.html` |
| **04** | **El equipo de ensueño** | [`t3/04 El equipo de ensueño.html`](t3/04%20El%20equipo%20de%20ensue%C3%B1o.html) | `https://pfelipm.github.io/uji-vj1224/t3/04%20El%20equipo%20de%20ensue%C3%B1o.html` |
| **05** | **Factores de éxito** | [`t3/05 Factores de éxito.html`](t3/05%20Factores%20de%20%C3%A9xito.html) | `https://pfelipm.github.io/uji-vj1224/t3/05%20Factores%20de%20%C3%A9xito.html` |
| **06** | **Auditoría del backlog** | [`t3/06 Auditoría del backlog.html`](t3/06%20Auditor%C3%ADa%20del%20backlog.html) | `https://pfelipm.github.io/uji-vj1224/t3/06%20Auditor%C3%ADa%20del%20backlog.html` |
| **07** | **Scrum of Scrums** | [`t3/07 Scrum of Scrums.html`](t3/07%20Scrum%20of%20Scrums.html) | `https://pfelipm.github.io/uji-vj1224/t3/07%20Scrum%20of%20Scrums.html` |
| **08** | **Scrum Lego city** | [`t3/08 Scrum Lego city.html`](t3/08%20Scrum%20Lego%20city.html) | `https://pfelipm.github.io/uji-vj1224/t3/08%20Scrum%20Lego%20city.html` |

---

### 📐 Temas 4, 5 y 6. Modelado de videojuegos con UML (DCU, DC y DA)

| # | Píldora interactiva (SPA) | Archivo local | URL directa (GitHub Pages / Google Sites) |
| :-: | :--- | :--- | :--- |
| **01** | **El mapa del modelado** | [`t4-t5-t6/01 El mapa del modelado.html`](t4-t5-t6/01%20El%20mapa%20del%20modelado.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/01%20El%20mapa%20del%20modelado.html` |
| **02** | **De Agile a UML** | [`t4-t5-t6/02 De Agile a UML.html`](t4-t5-t6/02%20De%20Agile%20a%20UML.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/02%20De%20Agile%20a%20UML.html` |
| **03** | **Los pilares del diseño** | [`t4-t5-t6/03 Los pilares del diseño.html`](t4-t5-t6/03%20Los%20pilares%20del%20dise%C3%B1o.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/03%20Los%20pilares%20del%20dise%C3%B1o.html` |
| **04** | **Guía rápida DCU** | [`t4-t5-t6/04 Guía rápida DCU.html`](t4-t5-t6/04%20Gu%C3%ADa%20r%C3%A1pida%20DCU.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/04%20Gu%C3%ADa%20r%C3%A1pida%20DCU.html` |
| **05** | **Arquitecto de blueprints** | [`t4-t5-t6/05 Arquitecto de blueprints.html`](t4-t5-t6/05%20Arquitecto%20de%20blueprints.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/05%20Arquitecto%20de%20blueprints.html` |
| **06** | **Los actores del juego** | [`t4-t5-t6/06 Los actores del juego.html`](t4-t5-t6/06%20Los%20actores%20del%20juego.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/06%20Los%20actores%20del%20juego.html` |
| **07** | **Guía rápida DC** | [`t4-t5-t6/07 Guía rápida DC.html`](t4-t5-t6/07%20Gu%C3%ADa%20r%C3%A1pida%20DC.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/07%20Gu%C3%ADa%20r%C3%A1pida%20DC.html` |
| **08** | **Guía rápida DA** | [`t4-t5-t6/08 Guía rápida DA.html`](t4-t5-t6/08%20Gu%C3%ADa%20r%C3%A1pida%20DA.html) | `https://pfelipm.github.io/uji-vj1224/t4-t5-t6/08%20Gu%C3%ADa%20r%C3%A1pida%20DA.html` |

---

## 🗺️ Próximos temas en desarrollo

- **Tema 7:** Planificación económica, presupuesto y contratación en el desarrollo de videojuegos.

---

## 📄 Licencia y autoría

© 2026/2027 **Pablo Felip Monferrer** · Departamento de Lenguajes y Sistemas Informáticos · **Universitat Jaume I (UJI)**.  
Estos materiales docentes se distribuyen bajo una licencia **[Creative Commons Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)](LICENSE)**.
