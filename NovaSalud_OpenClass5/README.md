# NovaSalud | Del piloto al servicio — Open Class 5 (UTEL)

Sitio estático **100 % local**: `index.html`, `styles.css`, `app.js`. Sin CDN, dependencias, cuenta de usuario ni backend. El caso es didáctico y **no se usa para tomar decisiones médicas**.

## Ejecutar con VS Code y Live Server
1. Abrir esta carpeta con VS Code.
2. Abrir `index.html` con **Open with Live Server**.
3. Realizar las 7 pantallas del recorrido. Los formularios guardan información en `localStorage` del navegador.
4. Al terminar, seleccionar **Descargar TXT** o **Imprimir / Guardar PDF** (opción Guardar como PDF del navegador).

## Publicar en GitHub Pages
Subir `index.html`, `styles.css`, `app.js` a la raíz de un repositorio. Settings → Pages → Deploy from a branch → main → /(root). Las respuestas siguen guardándose **solo en el dispositivo** de cada alumno; GitHub Pages no recibe ni centraliza datos. Para recibir entregables, solicítalos en tu plataforma institucional.

## Propósito y fuentes
Se basa en la presentación Open Class Semana 5 y la consigna del notebook OPEN-S05. Su reto central: evaluar condiciones para integrar un modelo de apoyo a la priorización de pacientes en un servicio hospitalario. Se respetan cuatro dimensiones de investigación: **Datos, Interoperabilidad, Tiempo real, Mejora continua**. Arquitectura y orquestación están presentes en el análisis transversal.

Repositorio opcional: https://notebook.google.com/notebook/d0f5cf8d-1b4d-4fdb-84e3-9b05d4f7550c

No se descargan automáticamente las fuentes de NotebookLM. Cada estudiante documenta su evidencia y debe comprobar sus citas. Si el notebook no está accesible, puede usar referencias de la presentación, consignando evidencia pendiente de verificar. El sitio contiene orientaciones conceptuales, NO textos ni citas de las fuentes originales.

## Recorrido
1. **El encargo:** introduce el escenario de NovaSalud.
2. **Cuatro incidentes:** explorar respuestas y consecuencias de problemas en datos, interoperabilidad, tiempo real y mejora continua.
3. **Hipótesis:** elegir la dimensión crítica y justificar la hipótesis.
4. **Investigación:** documentar dos fuentes diferentes y cuatro campos por fuente (fuente, hallazgo, interpretación, aplicación).
5. **Plan de acción:** causa → consecuencia → acción → resultado esperado; mecanismo de verificación.
6. **Contraste:** revisar condiciones transversales, escuchar otra perspectiva, revisar la hipótesis y emitir decisión.
7. **Dictamen:** vista previa, TXT UTF-8 y PDF por impresión.

## Uso docente sugerido
- Explicación de diapositivas 1–14 antes de abrir la web.
- Actividad central: 3 minutos para dimensión + hipótesis, 7 minutos para las dos evidencias, 6 minutos para plan de acción, 4 minutos para contraste y recomendación. La inspección de los cuatro miniincidentes puede hacerse como demostración guiada previa; así se mantiene el bloque de 20 minutos de las diapositivas.
- Socialización: solicitar a cada dupla una evidencia, un problema y una acción. La duración de la socialización depende del número de duplas.
- No interpretar la validación de longitud como evaluación automática de calidad ni el caso como una simulación clínica real.

## Pruebas recomendadas
- Seleccionar incidentes y verificar que la explicación cambie.
- Intentar avanzar sin respuesta y comprobar el aviso.
- Completar dos evidencias de fuentes diferentes.
- Completar cadena causal y comparar la decisión final con la hipótesis.
- Descargar TXT y comprobar acentos; usar impresión PDF.
- Reiniciar solo cuando se desee borrar el progreso local.

## Nota técnica
La funcionalidad de copiar una pregunta requiere permisos de portapapeles del navegador. Es opcional; el botón para abrir NotebookLM y la investigación manual permanecen disponibles.


## Cambios de la V2 (M01–M10)

- M01: Las opciones seleccionadas se califican visualmente al elegirlas: verde (control recomendable), ámbar (limitaciones), rojo (riesgo alto). No se indica la respuesta antes de seleccionar.
- M02: Instrucción clara de investigar **una sola dimensión**, después de explorar los cuatro incidentes.
- M03: Guía breve para formular la hipótesis.
- M04: Recomendaciones para trabajar con dos pestañas (sitio y NotebookLM).
- M05: Interpretación crítica de respuestas de NotebookLM, no copia automática.
- M06: Pregunta de investigación sin presuponer características técnicas no descritas en NovaSalud.
- M07: Consulta desplegable de las dos evidencias durante la elaboración del plan.
- M08: Consulta desplegable de evidencia, hipótesis y plan durante el contraste.
- M09: Modalidades de contraste por Zoom o individual con objeción del comité.
- M10: Dictamen TXT/PDF con siete apartados ordenados y sin encabezados duplicados.
- Cambio de redacción: «Propón» se reemplazó por «Formula» donde correspondía.

La V2 conserva la clave de almacenamiento local de V1 para facilitar continuar las pruebas en el mismo navegador y dirección de Live Server. Si se desea empezar desde cero, utilizar «Reiniciar». **No sustituye la verificación docente de fuentes y argumentos.**
