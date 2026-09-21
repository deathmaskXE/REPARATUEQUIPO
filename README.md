# Repara Tu Equipo · Recepcionador RTE

Sistema de recepción, seguimiento, agenda y notas PDF para **Repara Tu Equipo**.

## Categorías disponibles

- Consolas: imágenes en `assets/consolas/`.
- Controles: imágenes en `assets/controles/`.

La categoría Pantallas fue eliminada del selector, del catálogo y de los recursos.

## Notas PDF incluidas

- Confirmación de cita.
- Nota de recepción y anticipo.
- Nota de entrega y pago.

Las notas conservan la imagen ilustrativa del modelo seleccionado, sin QR ni firma.

## Agregar nuevos controles

1. Copia la imagen PNG a `assets/controles/` usando un nombre en minúsculas y sin espacios.
2. Abre `equipment-images.js`.
3. Dentro de `controllers.items`, agrega una entrada con nombre, archivo y términos de búsqueda.

Ejemplo:

```js
{label:"Control nuevo",file:"control-nuevo.png",terms:["control nuevo","modelo 1234"]}
```

## Configuración pendiente

Antes de publicar, completa:

- El Firebase exclusivo del negocio en `firebase-config.js`.
- Responsable, teléfono, dirección y redes en `DATOS_TALLER`, dentro de `admin.js`.
- Las políticas de devolución, garantía y plazo de recolección.

Este proyecto utiliza el Firebase exclusivo de Repara Tu Equipo para mantener sus expedientes separados y protegidos.
