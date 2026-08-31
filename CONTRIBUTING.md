# CONTRIBUTING

Circuito de calidad para cualquier cambio en el nucleo del Programa SOFIA (aplica igual a Albert y a cualquier agente/gemelo digital del pool: Router SOFIA, Cluster de Memoria/KDB, Gemelos Kore AVF, AVFrere Copiloto, AVFrereTestPiloto, Gestor de Academia, Orquestador de Silos).

## Circuito obligatorio

1. Issue con objetivo, alcance IN/OUT y riesgo antes de tocar codigo.
2. Rama propia por autor (agente o humano), nunca commits directos a main.
3. Pull Request con la plantilla EARS obligatoria (ver seccion siguiente).
4. CI en verde: lint, tests, escaneo de secretos.
5. Checklist de objeciones: minimo una antitesis documentada antes de aprobar.
6. Aprobacion de CODEOWNERS del modulo afectado.
7. Fusion solo tras 4, 5 y 6 en verde.

## Plantilla de PR (bloques EARS obligatorios)

Toda PR debe incluir estos 6 bloques en su descripcion:

1. Comprobado: hechos, fuentes y datos verificables.
2. No comprobado: lagunas, supuestos y limites.
3. Opciones consideradas (minimo dos si la importancia lo justifica).
4. Antitesis: la mejor objecion a este cambio.
5. Recomendacion: coste, riesgo, reversibilidad, condicion de salida.
6. Gate: que requiere aprobacion humana explicita, si aplica.

## Post-mortem

Toda PR fusionada que despues genera un incidente se etiqueta `postmortem` y produce un cambio correspondiente en este documento o en las reglas de CI, para que no se repita.

## Relacion con gobernanza

Este documento no decide que se activa en produccion, eso corresponde a GATE A/B/C (ADR-0005). Este documento garantiza que lo que llega a esa puerta ya paso un filtro de calidad tecnica verificable.
