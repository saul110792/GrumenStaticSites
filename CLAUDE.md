# Instrucciones para Claude Code

Este repo contiene 3 sitios estáticos (uno por carpeta) y un `render.yaml` que los publica como 3 Static Sites en Render.

## Tarea
1. Si no hay repo git: `git init -b main`, agrega todo y haz el commit inicial ("Sitios iniciales: Grupo Sólido, Sistemtec, Gioana").
2. Crea el repo en GitHub y súbelo: `gh repo create sitios-uniformes --private --source=. --remote=origin --push`.
   - Si `gh` no está autenticado, pide al usuario que ejecute `gh auth login` y espera.
   - Si el nombre ya existe, pregunta qué nombre usar.
3. Valida `render.yaml`: YAML válido, 3 servicios con `runtime: static`, y cada `staticPublishPath` apunta a una carpeta existente con `index.html`.
4. Si la Render CLI (`render`) está instalada y autenticada, úsala para validar el Blueprint; si no, no la instales sin preguntar.
5. Al terminar, indica al usuario el paso manual en Render:
   **Dashboard → New → Blueprint → elegir el repo `sitios-uniformes` → Apply**.
   Las URLs serán `https://<name>.onrender.com` (con sufijo si el nombre está tomado).

## Reglas
- No cambies el diseño de los HTML salvo que el usuario lo pida.
- Los valores marcados `TODO` (teléfonos/correos) son placeholders: pide los datos reales antes de publicar o deja claro que siguen pendientes.
- Si el usuario entrega logos, guárdalos como `logo.png` en la carpeta de cada sitio y reemplaza el `<svg>` del encabezado marcado con el comentario `Reemplaza`.
- Commits pequeños y descriptivos en español.
