# NovaData · Sala de decisiones — Open Class 4 (versión 3)

Sitio independiente de Gemini, creado para la dinámica de investigación de la Unidad 4 de UTEL. La versión 3 reorganiza las cinco rondas como una secuencia narrativa: **situación → evidencia → decisión → retroalimentación → transición y debate en Zoom**. Contiene matriz final y descarga TXT.

## VS Code y Live Server

1. Abre la carpeta `dist` en VS Code.
2. Haz clic derecho en `index.html` → **Open with Live Server**.
3. Navega en orden usando el único botón principal de cada pantalla. No hay navegación lateral para saltar pasos.
4. Completa la matriz de cinco criterios y descarga la ficha antes de reiniciar.

## GitHub Pages

Sube **el contenido de `dist`** (`index.html`, `styles.css`, `zoom.css`, `narrative.css`, `flow.js`) a la raíz de un repositorio. En **Settings → Pages**, configura publicación desde rama `main`, carpeta `/ (root)`. El archivo `app.js` corresponde a la versión 2 y ya no es necesario en la V3.

## Dinámica individual con discusión en Zoom (25 minutos)

1. **Minutos 0–4:** todos deciden individualmente la ronda 1. Cada uno copia `A/B/C · R1 · argumento breve` al chat de Zoom. El profesor comenta las posturas visibles.
2. **Minutos 4–10:** rondas 2 y 3. Pregunta quién cambió de postura y qué evidencia concreta le hizo cambiar.
3. **Minutos 10–17:** ronda 4. Contrasta la eficiencia defendida por la dirección con la supervisión propuesta por el comité de innovación.
4. **Minutos 17–22:** ronda 5 y matriz ejecutiva; cada estudiante formula su veredicto y su condición de supervisión.
5. **Minutos 22–25:** debate final. Cada estudiante registra una postura ajena y explica cómo modificó, fortaleció o complicó su razonamiento. Después descarga la ficha TXT.

La socialización de Zoom aparece junto a la retroalimentación, inmediatamente después de confirmar la decisión. El sitio no recopila ni cuenta respuestas de toda la clase. No hay saltos entre rondas ni dos botones principales simultáneos.

## Integración futura de Gemini

En la pantalla de cierre hay un botón **Copiar prompt para Gemini**. Es opcional: no depende de una Gem creada ni de claves API. El contraste crítico local ya funciona sin conexión a Gemini.

## Consideraciones docentes

- Se conserva la evidencia del caso: reducción del 30 % del tiempo, predicción de contracción fintech, señales humanas de recuperación, preocupaciones sobre interpretabilidad, ética, organización y gobernanza.
- Las decisiones y argumentos se guardan en `localStorage` del navegador del estudiante. No se recopilan en un panel docente ni se envían a servidores. La prueba de finalización es la ficha TXT descargada.
- La longitud mínima hace más difícil avanzar sin redactar, **pero no certifica la calidad del razonamiento**. La defensa oral y la discusión en clase siguen siendo necesarias.
- El archivo exportado identifica la progresión, la matriz y el veredicto. No constituye una calificación automática.
- Las pausas marcadas como completadas son declaraciones locales del estudiante, no comprobantes verificables de actividad en Zoom.
