# RESULTADOS DE TESTING - "SITIO-WEB-QA-TESTING"

## TEST 1: Validez HTML

* W3C Validator:

  * Criterio de éxito: Documento verde (Pass). Se aceptan máximo 3 warnings, pero 0 errores.
  * Resultado: Validacion Satisfactoria
  * "Document checking completed. No errors or warnings to show."

## TEST 2: Auditoría Accesibilidad (WAVE)

* Extensión WAVE para Chrome/Firefox.

  * Criterio de éxito: 0 Errores rojos. Las alertas amarillas son aceptables si están justificadas (máximo 5 alertas).
  * Resultado: 0 Errores Rojos, 0 alertas,  errores de contraste

## TEST 3: Estrés Responsive

* DevTools (F12) -> Device Mode.

  * Acción: Prueba en 3 anchos clave:
    * 320px (Móvil):
      [x] Sin scroll horizontal
      [x] Botones ≥48px
      [x] Texto ≥14px
      [x] Imágenes escalan
      [x] Navegación adaptada
    * 768px (Tablet):
      [x] Grid 2 columnas
      [x] Espaciado adecuado
    * 1440px (Desktop):
      [x] Grid 3 columnas
      [x] Max-width respe
      [x] Espaciado adecuado
    * 1440px (Desktop):
      [x] Grid 3 columnas
  * Resultado: Estilos responsivos responden de manera correcta

## TEST 4: Contraste de Color (WCAG)

* WAVE - Color Contrast Analyzer.

  * Acción: Mide el color del texto gris oscuro contra el fondo blanco y el azul de los enlaces.
  * Criterio de éxito: Ratio mínimo de 4.5:1 (AA).
  * Resultado: "No contrast errors were detected in the page. Manual testing is necessary to test for other potential contrast issues."
    * Contrast Ratio: 8.59:1
    * WCAG AA: Pass
    * WCAG AAA: Pass

## TEST 5: Navegación por Teclado (Focus)

* Tecla TAB.

  * Acción: Navega por toda la web sin usar el ratón.
    [x] Links
    [x] Buttons
    [x] Form inputs
    [x] Navigation items
  * Criterio de éxito: Debes ver siempre un recuadro (outline) azul grueso en el elemento seleccionado.
  * Resultado: Navega correctamente por todos lo elementos.

## TEST 6: Rendimiento (Lighthouse)

* DevTools -> Pestaña Lighthouse.

  * Acción: Genera un reporte en modo "Mobile".
  * Criterio de éxito: Puntuaciones verdes (>90) en Performance, Accessibility y Best Practices.
  * Resultado: Puntaje de 100 - Todos los elementos presentan rendimiento optimo
