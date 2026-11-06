# 📅 Agenda pública

Agenda interactiva hecha con HTML, CSS y JavaScript puro, sin dependencias ni instalación. Se publica gratis con GitHub Pages.

**Ver la agenda:** `https://santinomarceloe-creator.github.io/agenda_rl/`

## Qué puede hacer

- Calendario mensual con puntos de color según la categoría.
- Crear, editar, borrar y marcar eventos como hechos.
- Buscar por texto y filtrar por categoría.
- Vista por día o lista de próximos eventos.
- **Eventos compartidos:** se leen del archivo `eventos.json` y los ve cualquier visitante.
- **Eventos personales:** se guardan en el navegador de cada persona (`localStorage`) y se pueden exportar e importar como `.json`.
- Modo claro y oscuro automático.

## Estructura del proyecto

```
├── index.html     La página completa (estructura, estilos y lógica)
├── eventos.json   Eventos compartidos que ve todo el mundo
├── README.md      Esta portada
```
- [ ] Exportar a calendario (`.ics`)

## Licencia

Libre para usar y modificar. Si quieres una licencia formal, agrega una con **Add file → Create new file → LICENSE** y elige una plantilla (por ejemplo MIT).
