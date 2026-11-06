# 📅 Agenda pública

Agenda interactiva hecha con HTML, CSS y JavaScript puro, sin dependencias ni instalación. Se publica gratis con GitHub Pages.

**Ver la agenda:** `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO`

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
└── GUIA.md        Explicación de GitHub y Markdown
```

## Cómo agregar un evento compartido

1. Abre `eventos.json` en GitHub y haz clic en el lápiz ✎.
2. Agrega un bloque antes del `]` final (sin olvidar la coma entre bloques):

   ```json
   {
     "titulo": "Taller de Git",
     "fecha": "2026-12-02",
     "hora": "17:00",
     "categoria": "estudio",
     "notas": "Traer laptop."
   }
   ```

3. Clic en **Commit changes**. En uno o dos minutos aparece en la página.

Categorías válidas: `trabajo`, `estudio`, `personal`, `otro`. La fecha usa el formato `AAAA-MM-DD`.

## Publicar con GitHub Pages

1. **Settings → Pages**.
2. En **Source**, elige **Deploy from a branch**.
3. Selecciona la rama `main` y la carpeta `/ (root)`, y guarda.

## Probarlo en tu computadora

Abrir `index.html` con doble clic funciona, pero el navegador bloquea la lectura de `eventos.json`. Para verlo completo, desde la carpeta del proyecto ejecuta:

```bash
python -m http.server 8000
```

y abre `http://localhost:8000`.

## Cómo contribuir

1. Haz un **fork** del repositorio.
2. Crea una rama, por ejemplo `agregar-evento-diciembre`.
3. Edita `eventos.json` y haz commit.
4. Abre un **Pull Request** explicando qué agregaste.

## Ideas para seguir mejorando

- [ ] Eventos que se repiten (semanales, mensuales)
- [ ] Recordatorios con notificaciones del navegador
- [ ] Vista semanal
- [ ] Exportar a calendario (`.ics`)

## Licencia

Libre para usar y modificar. Si quieres una licencia formal, agrega una con **Add file → Create new file → LICENSE** y elige una plantilla (por ejemplo MIT).
