# Convencion de ramas (Batch C, integracion EARS)

Cada rama declara en que fase EARS esta el trabajo. Esto convierte la disciplina EARS en un artefacto tecnico inspeccionable, no solo en texto de Notion.

## Prefijos obligatorios

- `explore/nombre-caso` — fase Explorar. Objetivo, alcance IN/OUT, restricciones. Sin codigo funcional todavia, solo el issue vinculado y notas.
- `analyze/nombre-caso` — fase Analizar. Commits que separan hallazgo de hipotesis. Se referencia siempre al issue de `explore/`.
- `sandbox/nombre-caso` — fase Sandbox. Codigo ejecutable, pero SOLO contra el entorno de pruebas de CI (ver workflow), nunca contra produccion. El resultado de esta ejecucion se adjunta a la PR como evidencia, no se narra.
- Ramas sin prefijo (`feature/`, `fix/`, etc.) — trabajo directo que no requiere el ciclo EARS completo (cambios menores, correcciones de documentacion).

## Regla de oro

La fase Sandbox de EARS deja de ser "lo he probado, confia en mi" y pasa a ser un log de CI real, adjunto y verificable por cualquiera (incluido otro agente del pool). Ninguna PR que declare haber pasado por Sandbox se aprueba sin ese log adjunto.

## Relacion con CONTRIBUTING.md

Esta convencion es un desarrollo de la seccion "Plantilla de PR" ya existente en CONTRIBUTING.md — el bloque 1 (Comprobado) de esa plantilla debe enlazar al log de CI generado desde una rama `sandbox/`.
