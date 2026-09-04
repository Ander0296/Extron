# Checklist — "abro la app y NO me aparece el equipo en la lista"

Usalo cuando alguien (con computadora, celular o tablet) abre el
software de presentación inalámbrica y el receptor de la sala **no
figura** en la lista de equipos disponibles.

Ojo con el síntoma: esto NO es "pantalla negra". Acá la pantalla suele
estar bien, mostrando el fondo de espera del receptor. El problema está
en el camino de RED entre el dispositivo del usuario y el receptor.

Recorré los puntos EN ORDEN. Están de lo más barato y probable a lo más
caro y raro. Saltarse el orden es lo que hace perder horas.

## 1. Antes de tocar nada: mirá la pantalla de la sala

- [ ] ¿La pantalla muestra el fondo de espera del receptor?
      Si SÍ: el receptor está vivo y su salida de video anda. Ya
      descartaste alimentación, cable de video y pantalla. Seguí acá.
- [ ] Si la pantalla está NEGRA, este checklist no es el que va:
      el problema es de alimentación o de video, no de red.
- [ ] ¿La pantalla muestra el nombre del equipo y su dirección IP?
      Anotalos. Los vas a necesitar en el punto 4.

## 2. El dispositivo del usuario

- [ ] ¿Está conectado a la red? (Wi-Fi encendido, con red asociada.)
- [ ] ¿Está en la red CORRECTA? Muchos edificios tienen varias:
      la corporativa, la de invitados y la de los equipos. La de
      invitados casi nunca ve los equipos internos: está aislada a
      propósito.
- [ ] Si es celular o tablet: solo puede entrar por Wi-Fi. No tiene
      puerto de red, así que si el Wi-Fi de la sala no llega, no hay
      plan B por cable.
- [ ] ¿Tiene una VPN activa? Una VPN saca al dispositivo de la red
      local aunque el Wi-Fi diga "conectado", y entonces no descubre
      nada de la sala.

## 3. LA pregunta que resuelve la mitad de los casos

- [ ] ¿El dispositivo y el receptor están en la MISMA SUBRED?

      Estar en la misma red NO alcanza. El descubrimiento automático
      funciona porque el equipo "grita" que existe, y ese grito muere
      en el borde de su subred. Desde otra subred nadie lo escucha,
      aunque los dos tengan internet y todo funcione perfecto.

- [ ] Si están en subredes distintas: NO sigas buscando en la lista.
      Escribí la dirección IP del receptor a mano en la app (esa que
      anotaste en el punto 1). Es el camino previsto, no un truco.

## 4. La lista de la app

- [ ] ¿Refrescaste la lista? En móvil se arrastra hacia abajo y se
      suelta; en computadora hay un botón de refrescar o se reabre el
      diálogo de selección.
- [ ] ¿Probaste buscar por nombre de equipo Y por dirección IP? A veces
      el nombre está mal escrito o cambió y la IP sigue igual.
- [ ] Si aparece pero no conecta: mirá el código de acceso que muestra
      la pantalla de la sala. Si el equipo lo genera al azar, el código
      cambia solo y el que tenías guardado ya no sirve.

## 5. La red de la sala (acá ya llamás a redes)

- [ ] ¿El LED del puerto de red del receptor está encendido y
      parpadeando? Apagado = el cable o el puerto del switch.
- [ ] ¿Otro dispositivo en la misma sala lo ve? Si otro SÍ lo ve, el
      problema es del dispositivo del usuario, no del equipo.
- [ ] ¿El punto de acceso Wi-Fi de la sala está cableado a la misma red
      que el receptor? Si el Wi-Fi va a una red y el receptor a otra,
      nunca se van a ver, y todo lo demás puede estar impecable.

## Trampas conocidas

| Lo que parece | Lo que suele ser |
| --- | --- |
| "No hay red" | Hay red, pero es otra subred |
| "El equipo está roto" | El usuario está en la red de invitados |
| "La app anda mal" | Hay una VPN activa en el dispositivo |
| "Funciona a medias: algunas cosas sí y otras no" | Falta salida a INTERNET, no red local. Las funciones que traen contenido de afuera (nube, navegador) fallan; las que usan archivos del propio dispositivo andan bien |
| "Ayer conectaba y hoy no" | El código de acceso es aleatorio y cambió |

## La regla de fondo

**Red local e internet no son lo mismo, y red y subred tampoco.**

Un dispositivo puede tener internet perfecto y no ver el equipo de la
sala. Otro puede ver el equipo perfecto y no tener internet. Son tres
cosas distintas, y cada síntoma apunta a una sola. Antes de reiniciar
nada, decidí cuál de las tres te falta.
