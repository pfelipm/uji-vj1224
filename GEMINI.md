# Guía y convenciones del proyecto VJ1224

## 1. Estilo y maquetación de SPAs (HTML / Tailwind CSS)

### Sistema visual dual (Neobrutalismo en T1 y Retro-HUD de Alto Contraste en T2–T6)
* **Tema 1 (`t1/`)**: Estética neobrutalista oscura de alto impacto (`Space Grotesk` + `Space Mono`, bordes sólidos de `4px`/`5px` y sombras proyectadas sólidas `.brutal-box-*`).
* **Temas 2, 3 y 4–6 (`t2/`, `t3/`, `t4-t5-t6/`)**: Estética **Retro-HUD / Arcade Táctico de Alto Contraste** (`Press Start 2P` reservada para insignias HUD, contadores y titulares cortos; `Rajdhani` en pesos 600–700 para lectura nítida en el proyector del aula). Bordes definidos (`2px solid`) y codificación cromática neón (cian, esmeralda, ámbar, carmesí, violeta) sobre fondo reticulado `#080c14`.
* **Controles de revelado progresivo (`.hud-dock`)**: Siempre integrados en el flujo natural del documento (nunca flotantes con `fixed` que tapen contenido en iframes), reubicados dinámicamente justo debajo del último bloque revelado (`class="hidden"` real para los pasos pendientes) y compatibles con navegación por teclado (`Espacio`, `ArrowRight`, `ArrowLeft`).
* **Secciones desplegables con `<details>` nativo**: En guías de referencia (como DCU, DC y DA), emplear `<details>` y `<summary>` nativos para permitir apertura/cierre de bloques manteniendo la búsqueda nativa en página (`Ctrl+F`).

### Listas y viñetas (sangría francesa)
* **Nunca usar `list-inside`** en listas desordenadas (`<ul>`) u ordenadas (`<ol>`) que contengan texto explicativo o párrafos que puedan saltar a una segunda línea, ya que coloca el marcador dentro del flujo de texto e impide la sangría francesa (las líneas secundarias quedan debajo de la viñeta).
* **Usar siempre posición exterior con padding (`list-disc list-outside pl-5` o `list-decimal list-outside pl-5`)** o bien elementos flexibles (`flex items-start gap-2`) con icono/marcador `shrink-0`. De este modo el texto de las líneas subsiguientes se alinea verticalmente por la izquierda con la primera línea.

## 2. Tipografía y redacción en español

### Capitalización (*Sentence case*)
* Seguir las normas ortográficas de la RAE: en títulos, subtítulos, encabezados (`<h2>`, `<h3>`, `<h4>`), etiquetas y descripciones de tarjetas, usar mayúscula únicamente en la letra inicial de la frase y en nombres propios, siglas o términos metodológicos canónicos (p. ej., *Scrum*, *Agile*, *Lean*, *Sprint*, *Product Owner*, *Scrum Master*, *Product Backlog*, *Sprint Backlog*, *INVEST*, *Definition of Done*, *Kanban*, *Planning Poker*, *Gherkin*, *UML*, *Notion*, *Unity*).
* Evitar la capitalización de estilo anglosajón (*Title Case*) que capitaliza cada sustantivo y adjetivo.
* Escribir siempre **«Scrum»** (nombre propio derivado del rugby) y nunca «SCRUM» en mayúsculas como si fuera un acrónimo.

## 3. Arquitectura de despliegue continuo (GitHub Pages + Google Sites)

* **Detección contextual de incrustación (`is-embedded`)**: Todas las SPAs incluyen en el `<head>` el detector ligero `if (window.self !== window.top) { document.documentElement.classList.add('is-embedded'); }`.
* **Ocultación de navegación entre páginas (`.hide-in-embed`)**: Las barras de retorno al índice general (`../index.html`) y navegación secuencial (`← Anterior` / `Siguiente →`) llevan la clase `.hide-in-embed` para mostrarse cuando se navega desde GitHub Pages y ocultarse automáticamente al insertarse por URL a página completa en Google Sites.
* **Portapapeles con *fallback* compatible con iframes**: Cualquier función de copiado al portapapeles debe implementar `navigator.clipboard.writeText` con *fallback* automático mediante `document.execCommand('copy')` para sortear las restricciones de `Permissions-Policy` en Google Sites.
