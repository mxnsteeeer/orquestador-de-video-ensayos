# Video-Ensayo Orchestrator v3 — Orquestación completa

Orquestador de agentes especializados en video-ensayos serios para opencode.

Intención: conciencia vestida de lúgubre. Semilla pequeña, nunca sermón, nunca deprimir. Estructura similar, texto siempre nuevo, sin jerga en narración.

Ya no es solo guiones. Es canal completo: packaging + guion + crítica pros/contras + miniatura + SEO + horarios + calendario.

## Instalación (Omarchy)

Copia `.opencode/` a tu proyecto, reinicia opencode.

```
cp -r orquestador-de-video-ensayos/.opencode tu-proyecto/
cp orquestador-de-video-ensayos/ideas.md tu-proyecto/
cp -r orquestador-de-video-ensayos/calendario tu-proyecto/
cp -r orquestador-de-video-ensayos/templates tu-proyecto/
```

Fix v3 incluido: agentes ya apuntan a `SKILL.md` (no a `FORMATO.md` roto), UTF-8 limpio.

## Uso

```
/video-ensayo ideas
/video-ensayo Lapidación y castigos
```

Flujo v3:
FASE 1 packaging (empaquetador + seo + miniaturista) → FASE 2 guion (escritor + critico pros/contras) → FASE 3 edición+SEO (cinematografo + seo final + miniatura final + productor) → FASE 4 calendario (programador con horarios LATAM).

## Agentes

- `ideador` — vestido / semilla scoring
- `empaquetador` — director packaging: 3 títulos <60 chars + dirección miniatura
- `miniaturista` — miniaturas serias A/B + prompt IA + layout 1280x720
- `estratega-seo` — descripción poética + 40-50 tags + timestamps + comentario fijado
- `escritor` — guion serio, 3 círculos completos, semilla sin nombrar
- `critico` — VEREDICTO + 3 puntos a favor + 3 en contra con fix + tabla 0-10, exige >=7
- `cinematografo` — edición lenta 6-10s, desaturado, drone, shotlist
- `productor` — checklist tú-solo-narras
- `programador` — horarios subida LATAM, calendario editorial, cadencia 1/14 días, métricas 48h

## Estructura formato

1. HOOK 2 frases + 15s silencio
2. Pregunta marco
3. 3 bloques: abre → contexto con fechas/nombres/lugares → cierra
4. Espejo (barrio, familia, tú)
5. Semilla (3-4 frases rendija, 80% lúgubre + 20% luz, sin jerga)
6. Gracias por ver.

Ver `examples/`, `templates/`, `guiones/lapidacion-y-castigos-lectura.txt`, `calendario/editorial.md`.
