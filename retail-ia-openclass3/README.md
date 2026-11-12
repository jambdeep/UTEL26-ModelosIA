# Retail IA — Laboratorio de decisiones (versión 2)

Sitio estático para la Open Class 3 (Unidad 3), *Modelos de inteligencia artificial en negocios y servicios*, UTEL. Diseñado para trabajar sobre el caso transversal de una empresa retail que pronostica demanda y decide inventario.

## Abrir en Visual Studio Code

1. Abre la carpeta que contiene `index.html`, `styles.css` y `app.js`.
2. Abre `index.html` y usa **Open with Live Server**.
3. No se necesitan bibliotecas, internet, cuentas, ni servidor de aplicaciones.

## Publicar en GitHub Pages

1. Sube **los tres archivos** `index.html`, `styles.css` y `app.js` a la raíz de un repositorio de GitHub (puedes incluir este README).
2. En **Settings → Pages**, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
3. Abre la URL indicada en Pages. El sitio solo guarda resultados en la sesión actual del navegador y genera un archivo TXT local: no envía respuestas a un servidor.

## Mejoras incluidas en la versión 2

- **M01:** la evaluación de controles identifica específicamente las verificaciones omitidas.
- **M02:** umbral de alerta de error MAPE ajustable (datos ficticios) y señales interpretadas.
- **M03:** explicación cuando hay reposición calculada pero no se cumple la regla de inventario mínimo.
- **M04:** diferencia explícitamente una restricción por presupuesto pendiente.
- **M05:** explicación específica de la excepción por perecibilidad.
- **M06:** historial ampliado y comparación seleccionable de dos escenarios, con indicadores y reglas.
- **M07:** la ficha recoge resultados y diagnósticos del último escenario.
- **M08:** advierte sobre etapas incompletas, sin bloquear descarga.
- **M09:** avisa si la elección final de «implementar» contradice restricciones detectadas.
- **M10:** avisa si no se registraron dos fuentes externas (sin verificar su calidad automáticamente).
- **M11:** permite sustituir **demanda ajustada** y **compra propuesta** para crear una hipótesis alternativa; calcula inventario final y cobertura hipotética, manteniendo separados los resultados originales de las reglas y la autorización.

## Prueba rápida

1. En `2. Modelo + reglas`, marca una, tres y cuatro casillas: debe cambiar la retroalimentación.
2. En `3. Adaptación`, cambia el umbral MAPE de 12 a 20: se modifican las semanas que superan el umbral.
3. En `4. Simulador`, ejecuta el escenario base (demanda 1,200, compra calculada 400, revisión humana).
4. Cambia inventario a 150 y ejecuta (demanda 1,200, compra calculada 1,250, reposición sugerida).
5. Desmarca presupuesto y ejecuta (1,250 calculadas, pero revisión humana por presupuesto).
6. Reactiva presupuesto, marca perecedero y ejecuta (revisión por perecibilidad).
7. Selecciona dos escenarios en «Compara escenarios» y pulsa «Comparar».
8. En «Experimento M11», modifica demanda ajustada y compra propuesta: deben cambiar la cobertura y el inventario final **sin** cambiar el resultado calculado original.
9. En `5. Decisión`, genera la ficha con y sin fuentes externas. Verifica las advertencias, la vista previa y la descarga TXT (UTF-8 con BOM para mayor compatibilidad).

## Alcance y límites

- El +20 % de pronóstico y las situaciones de promociones, canales y competencia proceden del caso de la sesión. Los inventarios, fórmulas, umbrales y datos de desempeño son **supuestos didácticos**.
- La expresión de reposición es `max(0, demanda ajustada + inventario mínimo − inventario disponible)`.
- La reposición automática propuesta exige simultáneamente las cinco reglas didácticas. Estas reglas **no sustituyen políticas reales, revisión humana ni aprobación presupuestaria**.
- El experimento M11 utiliza una demanda y una cantidad de compra **impuestas por el estudiante**, y no vuelve a calcular la autorización automática a partir de estos datos; esto es intencional para diferenciar hipótesis de autorización.
- Los datos y decisiones se reinician al recargar el sitio; descarga la ficha antes de cerrar.
