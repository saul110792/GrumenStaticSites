# Sitios web – comercializadoras de uniformes

Tres landing pages estáticas (HTML + CSS, sin build) desplegadas en Render como Static Sites independientes.

| Carpeta | Empresa | URL esperada |
|---|---|---|
| `grupo-solido/` | Grupo Sólido Empresarial | https://grupo-solido.onrender.com |
| `sistemtec/` | Sistemtec | https://sistemtec.onrender.com |
| `gioana/` | GIOANA | https://gioana.onrender.com |

> Si el nombre ya está ocupado en Render, la URL llevará un sufijo. Cambia `name` en `render.yaml` para elegir otro.

## Despliegue
1. Sube este repo a GitHub.
2. En Render: **New → Blueprint** → selecciona el repo → **Apply**.
3. Render crea los 3 sitios. Cada uno solo se redespliega cuando cambian archivos de su carpeta (`buildFilter`).

## Pendientes por sitio
- Logo oficial: reemplazar el SVG del encabezado (comentario `Reemplaza`) por `<img src="logo.png">` y guardar el archivo en la carpeta del sitio.
- Teléfono y correo de Grupo Sólido y Sistemtec (buscar `TODO`).
- Los formularios de Grupo Sólido y Sistemtec usan `mailto:`; considerar Formspree o EmailJS.
- Confirmar dirección de Sistemtec ("Pedregal de Santo Domingo").

## Dominio propio
Render → sitio → Settings → Custom Domains → agregar el dominio y crear el CNAME que indique Render. SSL automático.
