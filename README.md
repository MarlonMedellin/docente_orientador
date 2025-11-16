# Profe Orientador 7° – Hojas de Vida SIEE

## Resumen integral del proyecto
“Profe Orientador 7° – Hojas de Vida SIEE” es un GPT personalizado que apoya a docentes de instituciones educativas públicas de Medellín en la redacción de hojas de vida para estudiantes de grado séptimo. Automatiza y estandariza los tres bloques institucionales (Aspectos Relevantes, Aspectos para Mejorar y Compromiso de la Familia) con lenguaje pedagógico, ético y humanizado alineado al SIEE.

## Impacto educativo y administrativo
- Reduce carga operativa docente y asegura coherencia institucional en los informes.
- Mejora la comunicación con las familias al ofrecer retroalimentaciones claras y constructivas.
- Fortalece la gestión institucional al mantener los criterios del SIEE en cada entrega.
- Humaniza la evaluación destacando procesos, avances y corresponsabilidad familiar.

## ¿Cómo funciona?
### Entradas que aporta el docente
Notas por asignatura, promedio semestral, asignaturas aprobadas/reprobadas, comportamientos y convivencia, información familiar y semestre a generar. El sistema solo usa los datos proporcionados (no inventa ni extrapola información).

### Proceso de generación
Las instrucciones del sistema y los archivos de conocimiento definen el tono, los criterios SIEE y las recetas de redacción. El modelo clasifica notas, identifica áreas altas (≥4.0) y bajas (<3.5), interpreta el promedio y aplica reglas de lenguaje profesional descritas en los archivos 01–06.

### Estructura de salida
Cada semestre se redacta en tres párrafos (~80 palabras c/u) y la respuesta se entrega en una **tabla HTML** con una fila y tres columnas, en este orden:
1. **Aspectos Relevantes**: en la columna “ASPECTOS RELEVANTES – PRIMER/SEGUNDO SEMESTRE” se incluye el párrafo que nombra asignaturas con desempeño alto/superior, interpreta el promedio y reconoce fortalezas académicas, actitudinales y convivenciales.
2. **Aspectos para Mejorar**: en la columna “ASPECTOS PARA MEJORAR – PRIMER/SEGUNDO SEMESTRE” se incluye el párrafo que lista todas las asignaturas con desempeño bajo (<3.5), indica cuántas son y recomienda acciones concretas. En el primer semestre, cuando exista al menos una asignatura en desempeño bajo, debe dejar explícito que el estudiante está reprobando el grado en ese momento, con tono orientador.
3. **Compromiso de la Familia**: en la columna “COMPROMISO DE LA FAMILIA – PRIMER/SEGUNDO SEMESTRE” se incluye el párrafo que convoca al acompañamiento respetuoso, reconoce apoyos existentes o solicita mayor corresponsabilidad.

## Directrices pedagógicas, didácticas y comunicacionales
- Evaluación formativa que prioriza reconocimiento de avances, claridad en propósitos y retroalimentación útil (Archivo 01).
- Lenguaje respetuoso, descriptivo y libre de etiquetas; describe comportamientos y procesos, nunca defectos personales (Archivos 01 y 04).
- Respeto por la diversidad, confidencialidad y alineación con la escala SIEE (Superior, Alto, Básico, Bajo).
- Enfoque constructivo y contextualizado para la comunidad educativa pública de Medellín.

## Directrices técnicas y límites operativos
- Nota mínima 3.5; toda nota <3.5 se considera desempeño bajo y debe listarse explícitamente (Archivo 02).
- Juicio global del promedio: ≥4.5 Superior, 4.0–4.49 Alto, 3.5–3.99 Básico aceptable, <3.5 Bajo.
- Humanidades integra Español + Inglés; Tecnología integra Tecnología + Informática + Emprendimiento.
- El modelo no inventa datos, no da diagnósticos, no contradice al docente ni genera semestres no solicitados.
- Se evitan plantillas mecánicas: los párrafos deben ajustarse al caso, manteniendo ~80 palabras con recomendaciones viables.

## Arquitectura del conocimiento y archivos del repositorio
- `01_Marco_Pedagogico_Hojas_de_Vida_Grado7.md`: principios éticos, escala SIEE y estructura mínima de los informes.
- `02_Instrucciones_Operativas_y_Formatos_Generacion_HV_Grado7.md`: reglas obligatorias de entrada/salida, interpretación del promedio y guías por bloque.
- `03_Banco_de_Ejemplos_y_Plantillas_HV_Grado7.md`: plantillas modelo y frases sugeridas para distintos escenarios.
- `04_Recetas_Avanzadas_y_Casos_Especiales_HV_Grado7.md`: estrategias para comportamientos complejos, ausentismo, uso de dispositivos y riesgos de repitencia.
- `05_Plantillas_Especificas_Promedio_y_Desempeno.md`: combinaciones listas para cada rango de promedio y número de asignaturas bajas.
- `06_NEAE_y_Ajustes_Razonables_en_Hojas_de_Vida.md`: lineamientos para estudiantes con NEAE, uso de diagnósticos reportados y recomendaciones familiares.
- `LICENSE`: licencia CC0 1.0 Universal.

## Flujo sugerido de uso
1. Recopilar datos reales del estudiante y validarlos con el SIEE institucional.
2. Determinar semestre, promedio, asignaturas altas/bajas y situaciones convivenciales o familiares.
3. Invocar el GPT personalizado asegurando que los archivos 01–06 estén cargados como conocimiento referencial.
4. Revisar la respuesta generada, validar que cumpla las reglas (listas de áreas altas/bajas, conteos, tono, longitud) y ajustar si es necesario.
5. Compartir el informe con la familia y registrar observaciones institucionales respetando la confidencialidad.

## Manejo de casos especiales y NEAE
- Describir necesidades de apoyo usando los mismos términos del docente; nunca inventar diagnósticos.
- Integrar los apoyos y avances en Aspectos Relevantes, señalar necesidades en Aspectos para Mejorar y reforzar la alianza familia–escuela (Archivos 04 y 06).
- En casos de riesgo de repitencia o múltiples áreas bajas, enfatizar planes de refuerzo y corresponsabilidad sin lenguaje punitivo.

## Límites y buenas prácticas
- El modelo no rellena vacíos de información ni dicta sanciones.
- Evita juicios personales y lenguaje punitivo; todo reto se presenta como oportunidad de mejora.
- Mantiene coherencia entre semestres cuando el docente aporta antecedentes.
- Promueve recomendaciones específicas (tutorías, hábitos, acompañamiento emocional) alineadas con la evidencia entregada.

## Licencia
Este repositorio está publicado bajo la licencia **CC0 1.0 Universal** (ver `LICENSE`), por lo que el contenido puede reutilizarse y adaptarse libremente citando las buenas prácticas educativas descritas aquí.
