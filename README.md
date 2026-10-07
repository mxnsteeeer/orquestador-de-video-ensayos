# Orquestador de Videos v4 — Sistema de productividad, no clonación

Sistema completo para crear contenido: packaging + guion + crítica pros/contras + miniatura + SEO + horarios + calendario.

Filosofía v4: el MOTOR es común (fases, checklist, cerrar hilos), el ESTILO es tuyo. Nadie debe hacer videos como los míos. Cada persona define su voz en el setup y la orquestación trabaja para esa voz.

## Instalación en Windows (PowerShell)

Requisitos: Windows 10/11, git, opencode instalado.

```powershell
git clone https://github.com/mxnsteeeer/orquestador-de-video-ensayos.git
Copy-Item -Recurse orquestador-de-video-ensayos\.opencode .\tu-proyecto\
Copy-Item orquestador-de-video-ensayos\ideas.md .\tu-proyecto\
Copy-Item -Recurse orquestador-de-video-ensayos\calendario .\tu-proyecto\
Copy-Item -Recurse orquestador-de-video-ensayos\templates .\tu-proyecto\
Copy-Item -Recurse orquestador-de-video-ensayos\canal .\tu-proyecto\
```

Verifica: debes ver `.opencode\command\video-setup.md` y `.opencode\command\video-ensayo.md`.

## Instalación en Omarchy / Linux

```bash
git clone https://github.com/mxnsteeeer/orquestador-de-video-ensayos.git
cp -r orquestador-de-video-ensayos/.opencode tu-proyecto/
cp orquestador-de-video-ensayos/ideas.md tu-proyecto/
cp -r orquestador-de-video-ensayos/calendario tu-proyecto/
cp -r orquestador-de-video-ensayos/templates tu-proyecto/
cp -r orquestador-de-video-ensayos/canal tu-proyecto/
```

## Instalación en Opencode (ambos)

1. Copia `.opencode/` como arriba.
2. Reinicia opencode (cierra y abre).
3. Verifica comandos:
```
/video-setup
/video-ensayo ideas
```
Si no aparecen, revisa que `.opencode/command/` tenga los 2 `.md` y reinicia de nuevo.

## Setup — primera vez (obligatorio, 15 min)

No te saltes esto. Sin perfil, el sistema se niega a generar con el estilo de ejemplo.

```bash
/video-setup
```

Te hará 7 preguntas una por una (nicho, referentes, tono, prohibidos, estructura/duración, edición/miniatura, frecuencia). Puedes pre-rellenar en `templates/mi-estilo.cuestionario.md`.

Resultado: crea `canal/mi-canal.md` (privado, en .gitignore, no se sube). A partir de ahí TODOS los agentes leen tu perfil primero.

## Personalización — cómo funciona

Qué SÍ defines tú (tu voz):
- Nicho + 3 referentes + 3 adjetivos de tono + frase ejemplo tuya
- Lo prohibido (3 cosas que nunca harás)
- Estructura con tiempos y duración (ej: 8 min tutorial, no a fuerza 12 min lúgubre)
- Edición (ritmo, color, sonido, texto) y packaging (fórmula títulos + estilo miniatura)
- Frecuencia realista + días de grabación

Qué NO se personaliza (motor de productividad):
- Fases: packaging → guion → crítica >=7 → edición+SEO → calendario
- Regla: todo dato que abre se cierra en el mismo video
- Checklist tú-solo-narras, shotlist, tags + timestamps, métricas 48h

Si pides "igual que los tuyos", el configurador te frena y propone 2 variaciones propias. El ejemplo lúgubre vive solo en `canal/mi-canal.ejemplo.md` como referencia, prohibido copiarlo.

Para cambiar estilo después: `/video-setup` de nuevo o edita `canal/mi-canal.md` a mano.

## Uso diario

```
/video-ensayo ideas
/video-ensayo Tu tema aquí
```

## Agentes v4

- `configurador` — entrevista y crea tu perfil
- `ideador` — ideas en TU nicho/tono
- `empaquetador` — 3 títulos con TU fórmula
- `miniaturista` — miniaturas A/B en TU estilo
- `estratega-seo` — tags + timestamps + fijado
- `escritor` — guion en TU estructura/duración
- `critico` — VEREDICTO + 3 pros + 3 contras con fix, exige >=7
- `cinematografo` — shotlist en TU ritmo/color
- `productor` — checklist
- `programador` — horarios LATAM + calendario en TU frecuencia

Ver `examples/`, `templates/`, `guiones/lapidacion-y-castigos-lectura.txt`, `calendario/editorial.md`.
