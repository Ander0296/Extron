# PRÁCTICA #02 — Los conectores del panel trasero y qué pasa cuando falta uno

Tipo: CONECTORES Y SUS LÍMITES + CASO DE FALLA
Si te trabás: revisá la Sesión #02 de GUIA.md
Checklists: ToDo/leer-el-panel-de-un-equipo.md · ToDo/diagnostico-pantalla-negra.md

Resolvé TODO acá abajo, a mano, escribiendo debajo de cada consigna.
No mires el manual hasta terminar; después sí, para contrastar (eso es
el paso 2 de "probar" tu trabajo).

# ============================================================
# SEGURIDAD — leelo antes de empezar
# ============================================================
Esta práctica es 100% de escritorio: NO hay que tocar ningún equipo.
Si en algún momento se te ocurre ir a verificar algo en una sala real:
esa sala puede estar en uso, y un equipo en producción no se toca sin
autorización. Ante la duda, se practica por escrito.

# ============================================================
# PARTE A — La tabla de conectores
# ============================================================

El panel trasero del ShareLink 200 N tiene seis puntos, de la A a la F.
Sin mirar el manual, completá esta tabla de memoria. Si de alguno no te
acordás, escribí "no me acuerdo" — eso es información útil, inventar no.

| Letra | Nombre del conector | ¿Entrada o salida? | ¿Qué señal lleva? | ¿Digital o analógico? | ¿Lleva audio? |
| --- | --- | --- | --- | --- | --- |
| A |  |  |  |  |  |
| B |  |  |  |  |  |
| C |  |  |  |  |  |
| D |  |  |  |  |  |
| E |  |  |  |  |  |
| F |  |  |  |  |  |

Debajo de la tabla, contestá en una línea cada una:

A. Audio Out, salida, audio, analogico, si 
B. LAN, entrada, lleva datos, Digital, si
C. Conector HD 15 pines, salida, datos, analógico, no
D. HDMI, salida, datos, digital, si
E. USB, entrada, control, no sé, no 
F. Potencia, entrada, corriente, digital, no

A1. ¿Cuántas ENTRADAS de señal tiene este equipo, y cuál es?
Tiene 3 entradas de señal, Puerto LAN PoE, USB, y Potencia

A2. ¿Por qué un equipo que muestra video en una pantalla tiene una sola
    entrada, y encima no es de video?
No entendí

# ============================================================
# PARTE B — Las dos salidas de video
# ============================================================

B1. Escribí la diferencia entre la salida HDMI y la salida VGA
    (el manual la llama "15-pin HD connector" = conector HD de 15
    pines) en términos de: qué tipo de señal es cada una y qué
    transporta cada una.
La diferencia entre HDMI y VGA es que en el HDMI estoy transmitiendo datos de forma digital es decir unos y ceros
Adicional se transmite imagen y se transmite audio, por el caso contrario el VGA es una señal analógica y no 
transmite audio, solo video.

B2. Una sala tiene el ShareLink conectado a un proyector viejo por la
    salida VGA. El presentador comparte un video de YouTube. Se ve
    perfecto y no se oye nada. ¿Por qué? ¿Qué conector del panel
    trasero resuelve esto y a dónde tiene que ir el cable?
Esto pasa porque el VGA no transmite audio, debe haber un cable que va a la salida de audio Jack 3.5 del sharelink

B3. Escribí el camino completo del AUDIO en esa sala, una vez
    resuelto, con el formato "origen --medio--> destino".
El camino completo es el siguiente, 
Sale del portatil al access point via WiFi, del acces point se transporta al network via cable de red
de la network se transporta al sharelink 200 N por via cable de red.
Para transmitir el audio se debe conectar un cable con Jack 3.5 a la salida del sharelink

# ============================================================
# PARTE C — Alimentación (PoE)
# ============================================================

El manual dice, sobre PoE:

> "Power over Ethernet, or PoE, eliminates the need for a local power
> supply. Data and power are delivered over the single cable."
>
> (Traducción: "La alimentación a través de Ethernet, o PoE, elimina la
> necesidad de una fuente de alimentación local. Los datos y la
> corriente se entregan por el mismo único cable.")

C1. Explicá con TUS palabras qué implica técnicamente esa frase: qué
    cable deja de hacer falta y qué cable pasa a hacer dos trabajos.
El cable que deja de hacer falta es el de la potencia, ya que este va viajar a traves del cable de LAN PoE
Y se lo transmite un switche tenga esa caracteristica de poder transmitir potencia mediante Ethernet

C2. LA PREGUNTA QUE IMPORTA: un ShareLink alimentado por PoE está en
    una sala. El electricista corta la luz del cuarto de racks para
    hacer un trabajo, pero el enchufe de la sala de reuniones sigue
    con corriente. ¿El ShareLink sigue encendido? Explicá por qué.
El sharelink queda apagado, debido a que cortó la alimentación que viaja desde el switche.

C3. Estás delante de un ShareLink que no da señales de vida. ¿Cuál es
    la PRIMERA pregunta que hacés para saber si el problema es de
    alimentación, y por qué esa y no otra?
Primero miro el LED frontal, que me indica si tengo o no tengo potencia

# ============================================================
# PARTE D — Caso de falla, con el árbol ordenado
# ============================================================

Síntoma: en una sala, el televisor muestra la pantalla de espera del
ShareLink (o sea: el equipo está vivo y el HDMI llega bien). Un usuario
abre la app en su portátil y NO le aparece el ShareLink en la lista de
equipos a los que conectarse.

D1. Escribí el árbol de hipótesis ORDENADO, de la más probable / más
    barata de verificar a la menos. Una hipótesis por línea, y al lado
    QUÉ verificás para descartarla.
Revisión visual, primero revisamos que el led del puerto LAN, verificamos que esté encendido.
Revisar que el portatil esté conectado a la misma red del edificio.
Revision del access point
Revision del rack


D2. De todo el panel trasero, ¿qué conector es el sospechoso número
    uno en este síntoma, y cuál queda descartado de entrada? Justificá
    los dos.
Queda descartado el conector HDMI, el más sospechoso sería el cable LAN

# ============================================================
# CÓMO PROBAR TU TRABAJO ANTES DE ENTREGAR
# ============================================================
1. Recorré ToDo/leer-el-panel-de-un-equipo.md punto por punto sobre lo
   que escribiste. ¿Se te escapó alguno?
2. Recién AHORA abrí el manual (págs. 9 y 10 del PDF) y contrastá tu
   tabla de la Parte A. Anotá abajo qué corregiste.
3. Explicate en voz alta, sin mirar, la respuesta de C2. Si te trabás
   al decirla, es que no la entendiste todavía.

Qué corregí después de mirar el manual:


# ============================================================
# CUANDO TERMINES — copiá esta línea entera y pegala en el chat
# ============================================================

/entrega PRÁCTICA #02 — Los conectores del panel trasero del ShareLink 200 N — ejercicios/02-conectores-panel-trasero.md
