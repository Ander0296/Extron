# Checklist — leer el panel de un equipo Extron que no conozco

Se recorre cuando me paro delante de un equipo (o de la página del
manual que lo dibuja) y necesito saber qué hace y cómo está conectado.
No es para memorizar: es para ir tachando mientras miro.

## 1. Antes de tocar nada

- [ ] ¿La sala está EN USO? Si sí, no toco nada. Solo miro y anoto.
- [ ] Anoto el MODELO exacto tal como está serigrafiado en el chasis
      (ej: "ShareLink 200 N"). Sin el modelo exacto no puedo buscar el
      manual correcto: Extron tiene familias enteras con nombres casi
      iguales.
- [ ] Saco una foto del panel trasero CON los cables puestos, antes de
      desconectar nada. Es mi único "deshacer".

## 2. Separar entradas de salidas

- [ ] Marco cuáles conectores son ENTRADA (por ahí llega la señal) y
      cuáles son SALIDA (por ahí se va hacia la pantalla).
- [ ] Cuento: ¿cuántas entradas y cuántas salidas hay?
- [ ] Si el manual rotula un conector como "OUT" u "OUTPUT", es salida
      aunque el cable que sale de ahí vaya a un equipo que parece
      "anterior" en la sala. Manda el rótulo, no la intuición.

## 3. Por cada conector, tres preguntas

- [ ] ¿Es un conector de SEÑAL o de CORRIENTE? La corriente no es
      señal: no transporta información, no es digital ni analógica, y
      no cuenta como entrada ni como salida de señal. Separalo aparte
      antes de seguir.
- [ ] Si es de señal: ¿QUÉ lleva? — video, audio, datos de red,
      control, archivos.
- [ ] ¿DIGITAL o ANALÓGICO? — HDMI y DisplayPort son digitales;
      VGA ("15-pin HD connector" en Extron) y el jack de 3,5 mm son
      analógicos.
- [ ] ¿LLEVA AUDIO O NO? — HDMI sí. VGA NO. Si veo un VGA usado como
      salida principal, tiene que haber un cable de audio aparte; si no
      lo hay, ya sé por qué no se oye nada.

## 4. Alimentación (el punto que más se saltea)

- [ ] ¿Tiene conector de corriente propio, y está enchufado?
- [ ] ¿El puerto de red dice "LAN / PoE"? Entonces el equipo PUEDE
      estar alimentado por el cable de red, sin fuente. Si es así, el
      equipo depende del switch: se cae el switch, se apaga el equipo.
- [ ] Si va por PoE: ¿ESE PUERTO concreto entrega PoE? No alcanza con
      que el switch esté encendido. Un switch sin PoE pasa los datos
      igual pero no da corriente, y un switch PoE con el presupuesto
      de potencia agotado deja puertos sin alimentar sin avisar.
- [ ] Si hay fuente externa: ¿es la de Extron? Una fuente genérica con
      el mismo enchufe puede dar un voltaje distinto y romper el equipo.
- [ ] ¿El LED de encendido está verde? Si no, el problema es de
      alimentación y NO tiene sentido revisar video ni red todavía.

## 5. Antes de cerrar

- [ ] Anoto qué cable va a cada conector y hacia dónde va el otro
      extremo. Un panel sin ese dato es media ficha.
- [ ] Si cambié algo: ¿anoté el valor anterior ANTES de cambiarlo?
- [ ] Paso lo anotado a su ficha en `fichas/`.

## Trampas conocidas

| Lo que parece | Lo que es |
| --- | --- |
| "15-pin HD connector" | Es VGA. Extron casi nunca escribe "VGA" en las especificaciones. |
| Un puerto de red = solo datos | Si dice PoE, también lleva CORRIENTE. |
| HDMI y VGA son intercambiables | HDMI lleva video + audio; VGA lleva video y nada más. |
| USB en un equipo AV = para PC | Suele ser USB tipo A para pendrive, teclado o ratón: el equipo hace de anfitrión, no de periférico. |
| "Analógico" y "digital" se aplican a cualquier conector | Solo se aplican a los de SEÑAL. Un conector de corriente no es ninguna de las dos cosas. |
| Una salida de audio se enchufa a cualquier altavoz | Un jack de 3,5 mm da nivel de línea: no tiene fuerza para mover un altavoz pasivo. Necesita un amplificador o un altavoz autoamplificado. |
| El botón de reinicio es inofensivo | Devuelve a fábrica: se pierden IP, contraseñas y configuración. No es una práctica de aprendizaje. |
| El switch está encendido, así que da PoE | Son dos cosas distintas: puede no ser un switch PoE, o tener el presupuesto de potencia agotado. Los datos pasan y la corriente no. |
| El LED apagado se investiga junto con la red | El LED parte el diagnóstico en dos ramas y no se cruzan. Apagado = solo alimentación. Verde = alimentación descartada, ahora sí red. |
