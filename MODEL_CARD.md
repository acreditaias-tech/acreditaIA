# Model Card — AcreditaIA (conjunto de sistemas)
**Fecha:** 2025-09-10

## 1. Descripción
Tres sistemas: `support-bot` (atención al cliente), `marketing-analytics` (clasificación/resumen) y `anomaly-detector` (detección de anomalías).

## 2. Uso previsto
- Asistente a agentes humanos (no reemplazo total).
- Clasificación de contenido de marketing interno.
- Señalización temprana de anomalías en logs.

## 3. Datos
- FAQ y tickets (baja a media PII), campañas de marketing. Retención 12–18 meses. Minimización y anonimización cuando aplique.

## 4. Riesgos y controles
- Posibles alucinaciones y errores de clasificación.
- Controles: human-in-the-loop, máscaras de PII, evaluación semanal.

## 5. Métricas
- Latencia media 850 ms (support-bot). Escalado a humano ~7%. Revisión mensual de drift.

## 6. Limitaciones
- Ambigüedad extrema requiere derivación humana.
- Datos históricos sesgados pueden afectar resultados.

## 7. Contacto
Abra una incidencia (Issues) en el repositorio público.
