# REPASO DEL EXAMEN #01 — método de diagnóstico y subred

Programado para: 2026-09-07
Tipo: CASO DE FALLA + TRADUCCIÓN TÉCNICA + explicar con tus palabras

Si te trabás: revisá las Sesiones #02, #05 y #07 de GUIA.md
Checklists: ToDo/diagnostico-pantalla-negra.md · ToDo/no-aparece-el-equipo-en-la-app.md

Esto NO es una práctica nueva: son los cuatro puntos que se cayeron en
el examen del 2026-09-04. Se rehacen desde cero, sin mirar cómo los
contestaste esa vez y sin abrir el manual hasta terminar.

Resolvé TODO acá abajo, a mano, escribiendo debajo de cada consigna.

# ============================================================
# SEGURIDAD — leelo antes de empezar
# ============================================================
Este repaso es 100% de escritorio: NO hay que tocar ningún equipo.
Si se te ocurre ir a verificar algo en una sala real: esa sala puede
estar en uso, y un equipo en producción no se toca sin autorización.
Ante la duda, se practica por escrito.

# ============================================================
# PARTE A — Subred, las dos mitades
# ============================================================

A1. Explicale a alguien que no sabe nada de redes qué es una subred y
    por qué le importa en su trabajo. SIN usar ninguna de estas
    palabras: subred, subnet, red, IP, máscara, broadcast, dirección.
    Podés usar una analogía.

    Requisito: tu explicación tiene que dejar claras LAS DOS COSAS que
    pasan cuando dos equipos están en subredes distintas — qué deja de
    funcionar, y qué SÍ se puede hacer igual. Si solo explicás una de
    las dos, el repaso no está aprobado.


A2. Un usuario abre la app en su celular y el receptor de la sala no
    aparece en la lista. Ya verificaste que está conectado al Wi-Fi
    correcto de la empresa y que el receptor está encendido y
    mostrando su pantalla de espera.
    ¿Qué sospechás, cómo lo confirmás, y qué hacés para que ese
    usuario pueda presentar HOY?


# ============================================================
# PARTE B — El orden del diagnóstico
# ============================================================

B1. Escribí la REGLA que usás para ordenar hipótesis en un
    diagnóstico. En una o dos frases, con tus palabras.
    (Pista de formato, no de contenido: la regla tiene que servir para
    decidir cuál de dos hipótesis va primero, sin pensarlo mucho.)


B2. Antes de formular la primera hipótesis, ¿qué hacés? Escribí el
    paso previo y explicá en una línea por qué saltearlo sale caro.


B3. Un compañero te manda esta hoja de un montaje que hizo:

    > Sala 7A — montaje terminado
    > 1. Receptor inalámbrico instalado en el rack.
    > 2. Cable de red del receptor al switch, puerto 4.
    > 3. Salida HDMI del receptor al televisor de la sala.
    > 4. Punto de acceso Wi-Fi de la sala conectado a la red de
    >    invitados del edificio.
    > 5. Fuente de alimentación del receptor conectada al enchufe del
    >    rack.
    > 6. El cliente pide presentar desde portátiles Y desde celulares.

    Encontrá TODOS los errores. Uno por línea, con su consecuencia
    concreta al lado.
    Ojo: la trampa de este ejercicio es exactamente la misma que la
    del examen. Leé la hoja entera antes de escribir nada.


# ============================================================
# PARTE C — Sala en uso
# ============================================================

C1. Te llaman por un problema en una sala donde HAY UNA REUNIÓN EN
    CURSO. Hacé dos listas:

    LO QUE SÍ PUEDO HACER AHORA (al menos 3 cosas):


    LO QUE ESPERA A QUE LA SALA ESTÉ LIBRE (al menos 3 cosas):


C2. En una línea: ¿cuál es el criterio que separa una lista de la
    otra?


# ============================================================
# PARTE D — Traducción técnica
# ============================================================

D1. En la hoja de especificaciones de un equipo Extron, una salida de
    video figura como:

    > "15-pin HD connector"
    > (traducción literal: "conector HD de 15 pines")

    Contestá:
    a) ¿Con qué nombre lo conoce todo el mundo?
    b) ¿Qué significan exactamente esas dos letras, "HD"? No es lo que
       parece.
    c) ¿Qué consecuencia concreta tiene equivocarse con eso al leer
       unas especificaciones para una sala nueva?


D2. Un equipo llega, la imagen se ve en la pantalla, pero se congela y
    se hace bloques cada pocos segundos cuando el presentador pasa un
    video.
    ¿Este síntoma dice que algo está roto, o dice otra cosa? Explicá
    la diferencia y decí cuál es la PRIMERA acción a tomar.


# ============================================================
# CÓMO PROBAR TU TRABAJO ANTES DE ENTREGAR
# ============================================================
1. Recorré ToDo/diagnostico-pantalla-negra.md punto por punto sobre lo
   que escribiste, sobre todo la sección del Paso 1 y la regla de oro.
   ¿Hay algún punto del checklist que tu respuesta se saltea?
2. Recorré también ToDo/no-aparece-el-equipo-en-la-app.md sobre la
   Parte A.
3. Recién AHORA abrí el manual y contrastá la Parte D. Anotá abajo qué
   corregiste.
4. Explicate en voz alta, sin mirar, la respuesta de A1 completa. Si al
   decirla te falta una de las dos mitades, todavía no está.

Qué corregí después de mirar el manual y los checklists:


# ============================================================
# CUANDO TERMINES — copiá esta línea entera y pegala en el chat
# ============================================================

/entrega REPASO DEL EXAMEN #01 — método de diagnóstico y subred — ejercicios/repasos/r-examen01-metodo-y-subred.md
