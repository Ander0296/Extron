# GUÍA: equipos AV Extron — los manuales oficiales de Extron (PDF)

No asume conocimiento previo — la mantiene Claude Code sesión a
sesión. Cada sesión cubre una tanda del material (tamaño según formato:
6-10 páginas si vino como texto, 3-5 si vino como imágenes), explicada
en español y conectada con práctica hecha a mano.
Prácticas: ver EJERCICIOS.md.

## INICIO RÁPIDO

- Último punto estudiado: ShareLink 200 N User Guide, pág. 10 del PDF
  (Installation: paneles trasero, frontal e inferior). Siguiente:
  "Setting up the Standby Screen", pág. 11
- Última tanda: Sesión #02 (2026-09-01)
- PRÓXIMA SESIÓN: `/rename extron-s04`
  (el nombre de la sesión de Claude sale SIEMPRE de esta línea, no se
  calcula: es un contador distinto al de las tandas, porque una sesión
  de Claude puede cubrir 2-3 tandas. Claude la actualiza al cerrar.)
- Prácticas pendientes: #02 [~] corregida 1ª entrega, esperando la 2ª — repaso r1 de la #01 el 2026-09-05
- Último triage (`/pendientes`): nunca todavía
- Último examen (`/examen`): nunca todavía
- Entorno verificado: 2026-08-27 — pdftotext 26.08.0, zathura, ttyper OK

## VOCABULARIO (solo si el material está en otro idioma; una fila por término nuevo)

| Original (inglés)                    | Español | En una frase |
| ------------------------------------ | ------- | ------------ |
| Collaboration Gateway | pasarela de colaboración | La caja que recibe la imagen de varios dispositivos por red y la manda a UNA pantalla. |
| Network Version | versión de red | El equipo NO crea su propio Wi-Fi: se enchufa a la red que ya existe en el edificio. |
| Wireless Access Point (WAP) | punto de acceso inalámbrico | La antena Wi-Fi de la sala; el celular se conecta a ella, no al ShareLink. |
| Display device | dispositivo de visualización | La pantalla, TV o proyector: el final de la cadena de señal. |
| Safety Instructions | instrucciones de seguridad | Sección legal fija: riesgo eléctrico. WARNING = puede matarte, ATTENTION = puede romper el equipo. |
| WARNING | advertencia | Peligro para la PERSONA (descarga eléctrica). |
| ATTENTION / CAUTION | atención / precaución | Peligro para el EQUIPO (se daña o se destruye). |
| NOTE | nota | Información importante, sin peligro. |
| FCC Class A | clase A de la FCC | Equipo homologado para entorno COMERCIAL, no doméstico: puede interferir en una casa. |
| User Guide | guía de usuario | El manual completo del equipo (48 páginas en este caso). |
| Conventions Used in this Guide | convenciones usadas en esta guía | Sección que explica qué significa cada cartel del manual. |
| Specifications | especificaciones | Datos técnicos duros: resoluciones, consumo, medidas. |
| SIS (Simple Instruction Set) | conjunto simple de instrucciones | El "idioma" de comandos de texto con que se le dan órdenes a un equipo Extron. |
| EDID Minder | (nombre propio Extron) | Tecnología Extron que memoriza el EDID de la pantalla para que la fuente nunca se quede sin él. |
| Features | características | Lista de "qué sabe hacer" el equipo. Es publicidad ordenada: se lee para saber qué buscar después. |
| Outputs | salidas | Los conectores por donde SALE la señal hacia la pantalla o el amplificador. |
| 15-pin HD connector | conector HD de 15 pines | Es el VGA de toda la vida. Extron casi nunca escribe "VGA" en las especificaciones: escribe esto. |
| Power over Ethernet (PoE) | alimentación a través de Ethernet | Un solo cable de red lleva datos Y corriente: el equipo no necesita enchufe propio. |
| LAN (Local Area Network) | red de área local | La red del edificio: los cables y switches que conectan todo dentro del mismo sitio. |
| RJ-45 | (conector RJ-45) | El conector cuadrado del cable de red, con la lengüeta de plástico. El único conector de ENTRADA del ShareLink. |
| Female connector | conector hembra | El agujero, el que está en el equipo. El macho es la punta del cable que entra ahí. |
| Full screen / four-window display | pantalla completa / cuatro ventanas | Una fuente ocupando todo el televisor, o cuatro fuentes a la vez en cuadrantes. |
| USB type A | USB tipo A | El USB rectangular clásico. Acá sirve para pendrive, teclado o ratón. |
| Rear / Front / Bottom Panel | panel trasero / frontal / inferior | Las tres caras del equipo que el manual documenta con un dibujo y letras A, B, C... |
| Power LED | LED de encendido | La luz del frente. Verde = el equipo tiene corriente. Primer punto de diagnóstico, siempre. |
| Reset button | botón de reinicio | Botón hundido en el panel inferior: devuelve el equipo a fábrica. Se pulsa con un clip. |
| Air handling spaces / wall cavities | espacios de tratamiento de aire / cavidades de pared | Falso techo por donde pasa el aire acondicionado, o el hueco de un tabique. La fuente NO va ahí. |
| LPS / Class 2 power unit | fuente de potencia limitada / clase 2 | Categoría de fuente de alimentación que no puede entregar más corriente de la segura. |
| SNMP | (protocolo simple de gestión de red) | Sistema que permite vigilar desde un servidor si el equipo está vivo, sin ir a la sala. |
| Standby Screen | pantalla de espera | Lo que muestra el equipo cuando nadie está presentando: instrucciones para conectarse. |

============================================================

SESIÓN #01 — 2026-09-01 — ShareLink 200 N: preliminares + Introduction
(págs. 2, 3, 4 y 7 del PDF de 48 — ~8% del manual)
- Estructura FIJA de todo manual Extron: preliminares (seguridad, FCC,
  convenciones) → Introduction → Installation → Operation → Reference
  → Specifications. Saber esto permite ir directo a lo que se busca.
- Los 3 carteles del manual: WARNING = riesgo para la persona;
  ATTENTION = riesgo para el equipo; NOTE = dato importante sin riesgo.
- FCC Class A = equipo de entorno COMERCIAL. No es un dato de adorno:
  explica por qué estos equipos viven en salas de empresa.
- Qué ES el ShareLink 200 N: pasarela de presentación INALÁMBRICA.
  Entra imagen por la RED (Wi-Fi/Ethernet) desde PC, tablet o celular;
  sale por HDMI a UNA pantalla. Windows, macOS, Android e iOS.
- "Network Version" es la clave del modelo: NO genera su propio Wi-Fi,
  se integra a la red del edificio. Si la red falla, el equipo no sirve
  aunque esté encendido y sano.
- Cadena de señal (Figure 1): dispositivo → Wi-Fi → WAP de la sala →
  red → Ethernet → ShareLink 200 N → HDMI → pantalla. Dos tramos con
  naturalezas distintas: red (paquetes) y HDMI (video).
- La página de marcas registradas es un mapa del vocabulario Extron:
  ahí aparecen SIS, EDID Minder, DTP, XTP, Global Configurator.
- Nota del profe: el material vino como PANTALLAZOS, pero el PDF tiene
  texto seleccionable. Próxima tanda: descargar el PDF y extraerlo con
  `pdftotext` — 3-4 veces más barato y se lee con más precisión.
- Verificación: identificó bien el tramo de red por descarte (la
  pantalla de bienvenida prueba que el HDMI está sano). Corregido el
  matiz de "Network Version": no basta con que haya Wi-Fi, el
  dispositivo y el ShareLink tienen que estar en la MISMA red — el
  Wi-Fi de invitados aislado es el caso que rompe esa suposición.
- PRÁCTICAS CREADAS: #01 (trazado de señal del ShareLink 200 N).
- PRÓXIMO PASO: pág. 8 del PDF, sección "Features".

SESIÓN #02 — 2026-09-01 — ShareLink 200 N: Features + Installation (paneles)
(págs. 8, 9 y 10 del PDF — ~21% del manual)
- El panel trasero ES la cadena de señal hecha física: UNA entrada
  (RJ-45) y varias salidas (HDMI, VGA/15 pines HD, audio 3,5 mm, USB).
  Todo lo que entra al equipo entra por el cable de red.
- PoE: el mismo cable RJ-45 lleva datos Y corriente. Si el switch da
  PoE, la fuente sobra. Consecuencia de diagnóstico: un equipo alimentado
  por PoE se apaga si cae el switch, aunque el enchufe de la sala funcione.
- Dos salidas de video, dos mundos: HDMI (digital, lleva video + audio)
  y VGA/15 pines HD (analógico, video SOLO). Por eso existe el jack de
  audio de 3,5 mm: es la pareja obligatoria del VGA.
- 4-en-1 y 1-a-4 son cosas distintas: cuatro ventanas = 4 fuentes en UNA
  pantalla; "hasta cuatro unidades" = 1 PC hacia 4 ShareLink y 4 pantallas.
- Panel frontal: 2 USB tipo A (teclado/ratón, anotación) + Power LED
  verde. Panel inferior: botón de reinicio (clip, sin corriente, enchufar
  y mantener 10 s).
- Nota del profe: la caja ATTENTION de la pág. 10 está en inglés Y
  francés — es el MISMO aviso repetido, no dos avisos distintos.
- Nota del profe: la pág. 8 era texto puro y vino como pantallazo.
  Ese tipo de página va con `pdftotext`; el pantallazo se reserva para
  los dibujos de panel (págs. 9 y 10, donde sí estaba justificado).
- Verificación: ordenó bien el árbol de PoE (LED → cable → switch) e
  ignoró solo la pista falsa del enchufe de la sala. Corregido: el LED
  parte el diagnóstico en DOS ramas que no se cruzan (apagado = solo
  alimentación); "switch encendido" no es "el puerto entrega PoE"; y
  el cable de audio va de SALIDA del equipo a ENTRADA del amplificador.
- PRÁCTICAS CREADAS: #02 (conectores del panel trasero + caso de falla).
- PRÓXIMO PASO: pág. 11, "Setting up the Standby Screen".

============================================================
(ACÁ VAN LAS SESIONES — Claude agrega la SESIÓN #01 en la primera
clase y sigue numerando hacia abajo, una sección por sesión, usando
el formato CORTO de referencia del final del archivo. Cuando este
archivo supere ~500 líneas, Claude mueve las sesiones viejas a
GUIA-ARCHIVO.md — ver la regla en CLAUDE.md.)
============================================================

# ============================================================
# FORMATO DE CADA SESIÓN (referencia para Claude — copiar y llenar)
# Formato CORTO obligatorio: 5-8 bullets, SIN bloques de código ni
# contenido repetido del chat (eso ya vive en el chat, el material y
# los archivos de práctica). Sin narrar las dudas (tema + veredicto
# en una línea). Máximo ~15 líneas por sesión.
# ============================================================

SESIÓN #NN — [fecha] — [tema] (punto exacto del material, % avance)
- [idea clave 1, una línea]
- [idea clave 2...]
- Ejercicios de la tanda: [nombre + pendiente/completado, o "ninguno"]
- Nota del profe: [solo si la hubo, una línea]
- Dudas: [tema + bien/corregido en una línea, o "ninguna"]
- PRÁCTICAS CREADAS: [#NN o "ninguna"]
- PRÓXIMO PASO: [una línea]
