# REPASO r1 — PRÁCTICA #01 — Trazado de señal del ShareLink 200 N

Programado para: 2026-09-05
Si te trabás: revisá la Sesión #01 de GUIA.md
Checklists: ToDo/diagnostico-pantalla-negra.md · ToDo/leer-el-panel-de-un-equipo.md

Esto es un REPASO: se hace DESDE CERO, sin abrir tu versión original ni
la corrección de aquella vez. El escenario es otro a propósito. Si no te
sale algo, escribí "no me acuerdo" — eso mide de verdad, inventar no.

# ============================================================
# SEGURIDAD
# ============================================================
Práctica de escritorio. No hay que tocar ningún equipo. Una sala en uso
no se toca, y un equipo en producción no se configura sin autorización.

# ============================================================
# EL ESCENARIO
# ============================================================

Sala de juntas del tercer piso. Hay un ShareLink 200 N en un mueble bajo
el televisor. El televisor está conectado por HDMI. La sala tiene su
propio punto de acceso Wi-Fi en el techo, cableado al switch del rack
de planta.

Una comercial entra con su portátil, abre la app y proyecta su
presentación. Funciona.

# ============================================================
# PARTE A — El camino
# ============================================================

A1. Escribí el camino COMPLETO que recorre la imagen desde la pantalla
    del portátil de la comercial hasta el televisor. Un salto por línea,
    en orden, con el formato:

        origen --medio--> destino

A2. Marcá en qué punto exacto de ese camino la imagen DEJA de ser video
    y pasa a ser otra cosa, y en qué punto vuelve a ser video.

A3. En una línea: ¿qué hace que eso sea posible, o sea, quién convierte
    la pantalla del portátil en lo que viaja por la red?

# ============================================================
# PARTE B — Los dos tramos
# ============================================================

B1. Ese camino se parte en dos tramos de naturaleza distinta. Nombralos
    y decí dónde está la frontera entre los dos.

B2. Por cada tramo, escribí una cosa que pueda fallar ahí y que NO pueda
    fallar en el otro.

# ============================================================
# PARTE C — Diagnóstico
# ============================================================

Al día siguiente, otro usuario en la misma sala: el televisor muestra la
pantalla de espera del ShareLink, pero él no consigue proyectar.

C1. Con solo ese dato, ¿qué tramo del camino queda DESCARTADO, y cuál
    es la prueba que lo descarta? Justificá.

C2. Escribí el árbol de hipótesis del tramo que queda, ORDENADO de lo
    más probable y más barato de verificar a lo menos. Una hipótesis
    por línea, y al lado QUÉ verificás para descartarla.

C3. De tu lista, señalá cuál es la causa más frecuente en la vida real
    y explicá en una línea por qué pasa tanto.

# ============================================================
# CÓMO PROBAR TU TRABAJO ANTES DE ENTREGAR
# ============================================================
1. Recorré ToDo/diagnostico-pantalla-negra.md punto por punto sobre lo
   que escribiste.
2. Contrastá tu camino contra el manual (Figure 1, pág. 7 del PDF) y
   anotá abajo qué corregiste. Este paso NO es opcional.
3. Explicate C1 en voz alta, sin mirar el papel.

Qué corregí después de mirar el manual:


# ============================================================
# CUANDO TERMINES — copiá esta línea entera y pegala en el chat
# ============================================================

/entrega REPASO r1 — PRÁCTICA #01 — ejercicios/repasos/r1-01-trazado-sharelink-200n.md
