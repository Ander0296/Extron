# CHECKLIST — Pantalla en negro / "no puedo presentar"

Recorré esta lista MIENTRAS diagnosticás, de arriba a abajo. No es para
memorizar: es para no arrancar por el final.

## Regla de oro, antes de tocar nada

- [ ] ¿La sala está EN USO? Si hay gente trabajando, no se toca nada.
      Se anota el síntoma y se resuelve cuando la sala esté libre.
- [ ] Antes de cambiar cualquier configuración, anotá el valor
      anterior. Sin eso no hay vuelta atrás.
- [ ] Si la sala está en uso y aun así te llaman, partí el trabajo en
      dos: MITIGAR ahora y DIAGNOSTICAR después.
      Mitigar = solo lo que no toca infraestructura ni cables: bajar un
      ajuste de calidad, mover a una persona de lugar, cambiar de
      entrada en el TV, reconectar la app.
      Diagnosticar = todo lo que implique tocar cables, conexiones,
      switches o configuración, y va cuando la sala esté libre.
      Por qué importa: revisar "un segundito" la conexión de un punto
      de acceso durante una reunión puede cortar esa reunión y todas
      las que cuelguen de ese equipo.

## Paso 0 — Escribí el camino de la señal ANTES de mirar el equipo

- [ ] Dibujá o escribí la cadena completa, paso por paso, de la fuente
      a la pantalla, con el medio de cada tramo (Wi-Fi, cable de red,
      HDMI).
      Por qué importa: cada flecha de ese camino es un lugar donde la
      señal se puede cortar. Sin el camino escrito, no estás
      diagnosticando: estás adivinando.
- [ ] Revisá la FORMA de cada línea: `origen --medio--> destino`. A cada
      lado de la flecha tiene que haber un EQUIPO (portátil, punto de
      acceso, switch, receptor, TV). Wi-Fi, cable de red y HDMI van
      SOBRE la flecha, nunca como una caja.
      Por qué importa: una lista de medios sueltos ("Wi-Fi -> Ethernet ->
      HDMI") no dice entre qué dos equipos está cada tramo, y entonces no
      sabés a qué equipo ir a mirar.

## Paso 1 — Separá SÍNTOMA de HIPÓTESIS

- [ ] Escribí el síntoma exacto, sin interpretarlo ("el TV está en
      negro", no "es el HDMI").
- [ ] Antes de formular UNA hipótesis: listá los datos que YA tenés a
      la vista y usalos. Lo que ves en la pantalla, los LEDs, lo que
      dice la hoja del montaje, lo que te contó quien llamó.
      Por qué importa: preguntar por algo que ya te contestaron cuesta
      una llamada, un viaje o una tarde. El dato servido es gratis.
      Primero se lee lo que hay; después se pregunta por lo que falta.
- [ ] Escribí varias hipótesis posibles, no una sola.
      Por qué importa: decir "está en negro, entonces es el HDMI" no es
      una hipótesis, es una conclusión sin prueba — y cierra la puerta
      a todos los demás tramos antes de haber mirado nada.

## Paso 2 — Mirá qué HAY en la pantalla (esto parte el problema en dos)

- [ ] ¿La pantalla está en NEGRO TOTAL, sin ningún cartel?
      → El problema está del equipo hacia la PANTALLA: alimentación,
      cable HDMI, entrada/fuente equivocada en el TV, TV apagado.
- [ ] ¿La pantalla MUESTRA algo (pantalla de bienvenida, instrucciones,
      código de conexión)?
      → El tramo HDMI está SANO, ya está probado. El problema está del
      equipo hacia ATRÁS: red, Wi-Fi, punto de acceso, el dispositivo
      de quien presenta.
      Por qué importa: este solo punto elimina la mitad del camino sin
      desenchufar nada.

## Paso 3 — Recorré el tramo que quedó, de a UNA cosa por vez

- [ ] Mirá los LEDs de estado del equipo antes que nada: alimentación y
      red. Un LED de red apagado ya te dice dónde mirar.
- [ ] Ordená lo que vas a revisar de lo MÁS BARATO Y COMÚN a lo más
      caro: primero lo que se mira sin tocar nada (entrada/fuente del
      TV, LEDs de estado, si el TV está encendido); después lo que
      exige desenchufar (probar otro cable HDMI); al final lo que
      exige permisos o herramientas (configuración de red, firmware).
      Por qué importa: una lista de hipótesis SIN ORDEN no es un plan.
      Si arrancás cambiando el cable HDMI, gastaste diez minutos y una
      escalera en lo que la mayoría de las veces era el TV en la
      entrada equivocada.
- [ ] Cambiá o probá UN elemento por vez y volvé a mirar el síntoma.
      Por qué importa: si cambiás dos cosas juntas y funciona, no sabés
      cuál era. No aprendiste nada y va a volver a pasar.
- [ ] ¿Le pasa a UNA persona sola o a TODAS? Si es una sola, el
      problema está en su dispositivo o en su red, no en la sala.
- [ ] ¿Está el dispositivo en la MISMA red que el equipo? Estar
      conectado al Wi-Fi no alcanza: la red de invitados suele estar
      aislada, y desde ahí no se ve el equipo.

## Si la imagen LLEGA pero llega MAL (se congela, hace bloques, se corta)

Este es otro síntoma, no el mismo. Si se ve algo, aunque se vea feo, el
camino completo EXISTE y ya está probado de punta a punta. No busques
cables sueltos ni equipos apagados: no es eso.

Acá el problema es de CAPACIDAD, no de existencia: la red no da abasto
para todo lo que se le está pidiendo.

- [ ] Bajá la calidad de imagen en el software de quien presenta
      (Normal en vez de Best). Es gratis, tarda segundos, lo hace el
      propio presentador y no toca ni un cable. Empezá SIEMPRE por acá.
- [ ] ¿El presentador está lejos del punto de acceso Wi-Fi, o hay
      paredes de por medio? Sugerí que se acerque. También es gratis.
- [ ] ¿Está pasando un video? El video en movimiento pide mucho más que
      una presentación de diapositivas. Que se vea bien la presentación
      y mal el video es coherente con falta de ancho de banda, no con
      un equipo roto.
- [ ] ¿Cuánta gente hay conectada a ese mismo Wi-Fi? Una sala llena
      compite por el mismo aire.
- [ ] Recién con la sala LIBRE: cobertura Wi-Fi, saturación de la red y
      conexiones del punto de acceso.

## Antes de dar el diagnóstico por cerrado

- [ ] ¿Podés decir en una frase QUÉ estaba cortado y POR QUÉ eso
      producía ese síntoma exacto?
- [ ] ¿Dejaste todo como estaba (valores anotados, cables como
      estaban)?

## Trampas conocidas

| Confusión típica | La diferencia real |
| --- | --- |
| "Está en negro = es el HDMI" | El negro total apunta al tramo HDMI/TV, pero solo si NO hay ningún cartel en pantalla. Con cartel, el HDMI ya está probado. |
| "Hay Wi-Fi, entonces hay red" | Estar en el Wi-Fi de invitados y ver el Wi-Fi de la sala no es lo mismo. Tienen que estar en la MISMA red. |
| Equipo encendido = equipo funcionando | El LED de alimentación solo dice que le llega corriente. El de red dice si está hablando con la red. |
| "Se ve mal, entonces algo está roto" | Si se ve algo, el camino entero funciona. Lo que falta es capacidad de red, no una pieza. Roto y saturado se arreglan distinto. |
| Síntoma vs causa | "No se ve" es el síntoma. La causa está en algún punto del camino: hay que recorrerlo, no adivinarlo. |
| "El receptor convierte todo" | Hay DOS conversores: la app en el dispositivo convierte la pantalla en datos de red, y el receptor de la sala convierte esos datos de vuelta en video HDMI. Si la app no convierte, al receptor no le llega nada. |
