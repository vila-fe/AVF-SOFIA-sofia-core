# AVF-SOFIA-sofia-core

**Repositorio de gobernanza InnerSource del Programa SOFIA Human-AI AVF.** No contiene el codigo de produccion del programa, es la capa de reglas, plantillas y puertas de calidad que se aplica sobre el codigo que vive en otros repositorios.

## Repositorios de codigo reales del Programa

- vila-fe/Sofia-Human-AI: servidor MCP para SOFIA Human AI v.3 (arquitectura HOTL + HITL, validacion PEARS)
- vila-fe/sofia-twin-digital-avf: Twin Digital AVF

## Que es InnerSource aqui

Aplicar la disciplina de codigo abierto interno (PRs, revision por pares, CI, propiedad por modulo) al desarrollo del Programa, con especial atencion al escenario de un pool de agentes/gemelos digitales concurrentes escribiendo codigo en paralelo (Router SOFIA, Cluster de Memoria/KDB, Gemelos Kore AVF, AVFrere Copiloto, AVFrereTestPiloto, Gestor de Academia, Orquestador de Silos).

Ver CONTRIBUTING.md para el circuito de calidad y CODE_OF_CONDUCT.md para las normas de interaccion.

## Mapeo de herramientas a roles InnerSource

| Herramienta | Rol InnerSource |
| --- | --- |
| Notion (MEM-KORE) | Registro maestro de decisiones y episodios |
| GitHub | Codigo, PRs, CI, revision por pares |
| Linear | Issues y seguimiento tecnico |
| Supabase | Backend versionado, StackGate-SOFIA |

## Gobernanza superior

Este repo no decide que se aprueba, eso sigue siendo GATE A/B/C (ADR-0005, Sintesis D de PROP-A24-19). Este repo garantiza que lo aprobado se ejecuta de forma verificable.

---
Creado 2026-08-31, Batch A del plan de integracion InnerSource.
