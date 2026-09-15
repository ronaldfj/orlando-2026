# Orlando 2026 · Itinerario con checklist

Itinerario interactivo para un viaje familiar a Universal Orlando (12–19 de octubre de 2026): una página HTML sin dependencias que se abre desde el celular y permite marcar cada actividad conforme se va cumpliendo.

**Abrir:** https://ronaldfj.github.io/orlando-2026/

## Qué incluye

- Una pestaña por día, más una pestaña "Antes" con lo que hay que resolver desde casa.
- Cada actividad tiene hora, casilla y notas (precios estimados, restricciones de altura, beneficios incluidos en el paquete).
- Barra de avance general y porcentaje por día.
- Se abre automáticamente en el día que corresponda durante el viaje.
- Se puede imprimir: cada día sale en su propia página.

## Cómo se guarda el avance

Las marcas se guardan con `localStorage` en el navegador del dispositivo donde se abre la página. Cerrar la pestaña o apagar el teléfono no las borra. Sí se pierden si se abre en modo incógnito o se limpian los datos del navegador. Cada dispositivo lleva su propia lista.

Recomendación: abrir la URL en el celular y usar "Añadir a pantalla de inicio" para que quede como una app.

## Editar

Todo está en `index.html`. Para cambiar una actividad, edita el texto dentro de su `<li>`. Para agregar un día, copia una `<section>` completa y cambia `data-day`, `data-label` y `data-sub`; las pestañas y el conteo se generan solos.
