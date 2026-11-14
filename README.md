# Caso 1 — Luciérnaga

Proyecto de Estudio y Diseño del Trabajo.

## Aplicación
- **Vista previa web:** https://raw.githack.com/VictorHugocervantes28/caso_1/main/app/index.html
- **Código fuente:** [app/index.html](app/index.html)

La vista previa usa un servicio externo para representar el HTML del repositorio. Si no carga, descarga app/index.html y ábrelo directamente en Chrome o Edge.

## Funciones incluidas
- Capacidad, demanda, faltante, coste equivalente e inventario.
- Registro de mediciones para método inicial y mejorado.
- Cronómetro de ciclos.
- Cálculo de tiempo normal y estándar por observación.
- Comparación de promedios y gráficos de barras.
- Resumen de carga por estación/recurso.
- Exportación de bitácora a CSV compatible con Excel y respaldo JSON.
- Criterios ergonómicos y fórmulas del caso.

## Datos y documentación
- documentos/punto-control.md: cálculos manuales, fórmulas, supuestos y discrepancias.
- documentos/extracto-datos-libro-original.json: extracto estructurado de los datos del libro original.
- documentos/validacion-adicional.md: discrepancias de valoración del elemento B.

## Privacidad y almacenamiento
Las mediciones se guardan en el almacenamiento local del navegador donde se usa la aplicación. No se envían automáticamente a GitHub ni a un servidor. Exporta CSV o JSON para respaldarlas o transferirlas a otro equipo.

## Límites importantes
- Los cálculos de capacidad son de régimen, no una simulación de producción real.
- La hipótesis de ajuste del ciclo del piloto B debe validarse con el anexo patrón del docente.
- Las cargas agrupadas por estación solo pueden interpretarse como utilización cuando las tareas son secuenciales y no se solapan.
- El Excel original debe añadirse manualmente a documentos/; el conector de esta sesión no adjunta archivos XLSX binarios.
