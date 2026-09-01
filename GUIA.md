# GUÍA: equipos AV Extron — los manuales oficiales de Extron (PDF)

No asume conocimiento previo — la mantiene Claude Code sesión a
sesión. Cada sesión cubre una tanda del material (tamaño según formato:
6-10 páginas si vino como texto, 3-5 si vino como imágenes), explicada
en español y conectada con práctica hecha a mano.
Prácticas: ver EJERCICIOS.md.

## INICIO RÁPIDO

- Último punto estudiado: ShareLink 200 N User Guide, pág. 7 del PDF
  (Introduction / About + Figure 1). Siguiente: "Features", pág. 8
- Última tanda: Sesión #01 (2026-09-01)
- PRÓXIMA SESIÓN: `/rename extron-s02`
  (el nombre de la sesión de Claude sale SIEMPRE de esta línea, no se
  calcula: es un contador distinto al de las tandas, porque una sesión
  de Claude puede cubrir 2-3 tandas. Claude la actualiza al cerrar.)
- Prácticas pendientes: #01 trazado de señal del ShareLink 200 N
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
