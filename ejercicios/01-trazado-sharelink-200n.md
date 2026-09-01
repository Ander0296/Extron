# PRÁCTICA #01 — Trazado de señal del ShareLink 200 N

Tipo: TRAZADO DE SEÑAL
Si te trabás: revisá la Sesión #01 de GUIA.md
Checklist: ToDo/leer-manual-extron.md

# ============================================================
# SEGURIDAD — LEER ANTES DE EMPEZAR
# ============================================================
Esta práctica es 100% POR ESCRITO. No hay que tocar ningún equipo,
ni conectar ni desconectar nada, ni entrar a ninguna interfaz web.
Si algún punto te dan ganas de "ir a mirarlo al equipo": los equipos
del edificio están EN PRODUCCIÓN. No se toca nada sin autorización, y
en una sala en uso no se toca nada. Punto.

# ============================================================
# ENUNCIADO
# ============================================================

ESCENARIO:
En una sala de reuniones del edificio hay un ShareLink 200 N. Una
persona entra con su portátil y quiere mostrar su pantalla en el
televisor de la sala, sin cables.

Resolvé TODO acá abajo, a mano, sin mirar el manual mientras escribís.
Cuando termines, recién ahí, contrastá contra el manual.

## PARTE A — El camino de la señal

Escribí el camino COMPLETO que recorre la imagen desde la pantalla del
portátil hasta el televisor. Uno por línea, en orden, y en cada paso
indicá por qué medio viaja (Wi-Fi, cable de red, HDMI...).

Formato sugerido (una flecha por paso):

1. ...
2. ...
3. ...
(los que hagan falta)

RESPUESTA A:
1. Wifi
2. Red
3. HDMI


## PARTE B — Los dos tramos

El camino que escribiste tiene dos tramos de naturaleza distinta.

B1. ¿Dónde está exactamente la frontera entre los dos? Nombrá el
    equipo donde termina un tramo y empieza el otro.

RESPUESTA B1: La frontera está en el sharelink, el primer tramo viaja hacia la network, el otro tramo hacia el display


B2. ¿Qué viaja por cada tramo? Explicalo con tus palabras, sin copiar
    del manual.

RESPUESTA B2:  En el primer tramo viajan datos desde un dispositivo via Wifi hacia la red, 
Luego por esa red, viajan esos mismos datos al sharelink por cable
El sharelink recibe esos datos y los transmite a un display por una salida de video, ya sea hdmi por ejemplo.



## PARTE C — "Network Version"

El nombre completo del equipo es "ShareLink 200 N Collaboration
Gateway – Network Version".

C1. ¿Qué implica esa palabra "Network" para poder usar el equipo? Es
    decir: ¿qué tiene que existir en la sala/edificio SÍ o SÍ para que
    alguien pueda presentar?

RESPUESTA C1: Debe existir una red o network en la que debe ir conectado el sharelink y el access point, esa red debe ser la misma para ambos para que se puedan comunicar desde un dispositivo a un sharelink.


C2. Consecuencia práctica: si mañana se cae el Wi-Fi del edificio pero
    el ShareLink está encendido, con su LED de red apagado y el HDMI
    bien conectado al televisor, ¿se puede presentar? ¿Por qué?

RESPUESTA C2: no se puede presentar ya que no tenemos comunicación entre el equipo y el sharelink.




## PARTE D — Diagnóstico

Un compañero te avisa: "en la sala 3 el televisor está en negro, la
gente no puede presentar con el ShareLink".

Escribí tu árbol de hipótesis ORDENADO: qué verificarías primero,
segundo, tercero... y POR QUÉ en ese orden. Mínimo 4 hipótesis.

Pista de método (no es la respuesta): pensá el camino de la Parte A y
recorrelo. Cada flecha de ese camino es un lugar donde la señal se
puede cortar.

RESPUESTA D:
Miramos si la sala está en uso.
Primero debemos saber si la pantalla está en negro total sin ningun cartel.
Si es el caso debemos mirar del equipo hacia la pantalla, puede ser potencia del equipo
cable hdmi, entrada o fuente equivocada, tv apagado.
Si tenemos una imagen en negro con carteles el del sharelink hacia atras y quiere decir que el tramo de hdmi está sano
en este caso revisamos los leds del sharelink, red, wifi, puntos de acceso, dispositivo de quien presenta.

## PARTE E — Traducción técnica

Traducí al español y explicá con tus palabras qué quiere decir esta
frase del manual (pág. 7):

  "To allow wireless connection, the ShareLink 200 N must be
   integrated into an existing network that has wireless capability."

RESPUESTA E: Significa que para que funcione el sharelink 200 N debe existir anteriormente una red que tenga capacidad inalambrica.
Es decir en el edificio tenemos un access point al que se puede conectar un portatil via WiFi,
La idea de todo es transmitir la pantalla de mi portatil por el televisor.
Para ello usamos el sharelink que es quien transforma los datos que enviamos por wifi y lo transforma en imagen que transmite el televisor,
Para que pueda ocurrir todo ese proceso debemos tener el sharelink y el ap conectados a la misma red.




# ============================================================
# CÓMO PROBAR TU TRABAJO (antes de entregar)
# ============================================================
1. Recorré el checklist ToDo/leer-manual-extron.md.
2. Contrastá contra el manual: buscá en el PDF si lo que escribiste
   coincide (págs. 7 y siguientes).
3. Equipo real: NO aplica en esta práctica. No toques nada.
4. Explicáte la Parte A en voz alta, sin mirar el papel, de corrido.
   Si te trabás en un paso, ese paso no lo entendiste todavía.

# ============================================================
# PROMPT DE ENTREGA (copiá esto cuando termines)
# ============================================================

/entrega PRÁCTICA #01 — Trazado de señal del ShareLink 200 N — ejercicios/01-trazado-sharelink-200n.md
