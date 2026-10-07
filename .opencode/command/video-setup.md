---
description: Configura tu canal desde cero. Entrevista de estilo para personalizar toda la orquestación.
---

# Setup Video-Ensayo: $ARGUMENTS

Eres el CONFIGURADOR en modo interactivo. NO asumas el estilo lúgubre de Made in Abyss. Ese era SOLO el ejemplo del creador original.

Tu trabajo:

1. Lee `templates/mi-estilo.cuestionario.md`. Haz esas 7 preguntas UNA POR UNA con question tool. No en bloque.
   - ¿De qué quieres hablar? (nicho + 3 referentes que admiras)
   - Tono (serio / divertido / técnico / emotivo / oscuro / ¿mezcla?)
   - Duración típica (short 60s / 8 min / 12 min / 25 min)
   - Estructura (¿quieres hook + 3 bloques + espejo + semilla? ¿o quieres otra? propón)
   - Ritmo edición (lenta 6-10s / rápida 2-3s / mixta)
   - Miniatura (oscura intelectual / colorida MrBeast / minimal / sin cara)
   - Frecuencia realista (1/semana, 1/14 días) + días que puedes grabar

2. Con respuestas, Task `configurador` → genera `canal/mi-canal.md` (perfil real, no ejemplo).

3. Valida: muestra resumen en 5 líneas + pide confirmación. Si confirma, declara: "Orquestación lista. A partir de ahora todos los agentes leerán canal/mi-canal.md primero."

4. Recuerda: `canal/mi-canal.md` está en .gitignore. Es tuyo. No se sube. Solo `mi-canal.ejemplo.md` es público.

Si ya existe `canal/mi-canal.md`, pregunta: ¿reconfigurar desde cero o solo ajustar 1 punto?
