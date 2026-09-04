# EJERCICIOS — equipos AV Extron

Este archivo guarda SOLO lo VIVO (se lee entero al inicio de cada
sesión, así que se mantiene corto a propósito):
- prácticas [ ] pendientes y [~] en curso
- repasos programados todavía no cumplidos
- la lista CONCEPTOS DOMINADOS

Todo lo CERRADO (prácticas [x] completadas con su corrección, repasos
ya cumplidos) lo mueve Claude a EJERCICIOS-ARCHIVO.md, que viaja por
git y NO se lee al inicio: solo consulta puntual.

Dos tipos de práctica: (A) DEL MATERIAL, las trae el libro/curso y el
usuario las intenta a mano ANTES de mirar la solución; (B) DEL PROFE,
las crea Claude al cierre de un tema o combinando 2-3 conceptos.
Toda práctica tiene su ARCHIVO DE ARRANQUE en ejercicios/ (lo crea
Claude: enunciado + prompt de entrega adentro, nada de solución).

Estados: [ ] pendiente  [~] en curso  [x] completada (fecha)
Corrección escrita en archivo: MÁXIMO 3 líneas. El detalle va al chat.

FORMATOS (referencia para Claude — copiar y llenar):

PRÁCTICA #NN — [tema] — [ ] pendiente
Tipo: (según los tipos definidos en el setup)
Arranque: ejercicios/... | Si te trabás: Sesión #Y de GUIA.md

MATERIAL — [nombre] — [tema] (punto del material, Sesión #Y) — [ ] pendiente
Arranque: ejercicios/... | Si te trabás: Sesión #Y de GUIA.md

REPASO — PRÁCTICA #NN (rX) — programado: AAAA-MM-DD — [ ] pendiente
Arranque: ejercicios/repasos/... (desde cero, sin mirar el original)

# ============================================================
# PRÁCTICAS ABIERTAS
# ============================================================

PRÁCTICA #02 — Conectores del panel trasero del ShareLink 200 N — [~] en curso (1ª entrega 2026-09-01)
Tipo: CONECTORES Y SUS LÍMITES + CASO DE FALLA
Arranque: ejercicios/02-conectores-panel-trasero.md | Si te trabás: Sesión #02 de GUIA.md
Checklists: ToDo/leer-el-panel-de-un-equipo.md · ToDo/diagnostico-pantalla-negra.md
Corrección 1ª entrega: BIEN B1, B2, C1, C2, C3 y el plano del audio (mejor que su texto).
MAL: confunde señal con corriente en la tabla A (marca la corriente como "digital"),
D1 ordenado por distancia física y no por probabilidad×costo, y saltó el paso 2 de probar.

# ============================================================
# REPASOS PROGRAMADOS (r1 ~3 días, r2 ~2 semanas, r3 ~1 mes)
# ============================================================

REPASO — EXAMEN #01, conceptos flojos — programado: 2026-09-07 — [ ] pendiente
Arranque: ejercicios/repasos/r-examen01-metodo-y-subred.md (desde cero)
Foco: (1) subred — las DOS mitades del concepto; (2) orden de diagnóstico y uso de
los datos ya visibles; (3) qué se puede y qué no con la sala en uso; (4) el término
"15-pin HD connector" del manual. (Sin respuestas acá: son las que se evalúan.)

REPASO — PRÁCTICA #01 (r1) — programado: 2026-09-05 — [ ] pendiente
Arranque: ejercicios/repasos/r1-01-trazado-sharelink-200n.md (desde cero, sin mirar el original)
Foco: escribir el camino de la señal en forma "origen --medio--> destino" y
ordenar las hipótesis de diagnóstico dentro de cada rama.

# ============================================================
# CONCEPTOS DOMINADOS (entran al graduarse una práctica con r3 bien)
# ============================================================

- (vacío por ahora)
