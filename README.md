# Rachas Diarias — web

Versión web estática de [Rachas Diarias](https://github.com/pblmza/rachas-diarias)
(app Flask local): **lectura 📖 · videojuego 🎮 · bajo 🎸**, 10 minutos al día.

**Web pública:** https://pblmza.github.io/rachas-diarias-web/

## Cómo funciona
- Un solo `index.html`: sin backend, sin dependencias, sin trackers.
- Los datos viven en el **localStorage del navegador** de cada dispositivo:
  nada sale de tu computador. Si abres la web en otro navegador o dispositivo,
  empieza vacía.
- Temporizador de 10 min por hábito que marca solo al terminar (sobrevive
  recargas). También se marca con un clic directo en la tarjeta.
- Semana lunes→domingo con fechas; **fin de semana opcional**: en blanco no
  rompe la racha (y no cuenta); un día de semana en blanco sí rompe.
- La racha sigue viva mientras hoy no esté cerrado en blanco.

## Alcance y límites
- Sin cuentas ni sincronización entre dispositivos por diseño: el registro de
  cada navegador es independiente.
- Para respaldar o mover datos: copia las claves `rachas_data_v1` y
  `rachas_timers_v1` del localStorage (DevTools → Application → Local Storage).