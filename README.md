# Cotizador CREO de Creer y Crear

Cotizador online de programas integrales para la comunidad educativa.

## Despliegue en Vercel (paso a paso)

### 1. Subir a GitHub

```bash
# En tu computador, crea una carpeta y copia el index.html y vercel.json
# Luego desde esa carpeta:

git init
git add .
git commit -m "cotizador creo inicial"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/cotizador-creo.git
git push -u origin main
```

### 2. Conectar con Vercel

1. Ve a [vercel.com](https://vercel.com) e inicia sesión con tu cuenta de GitHub
2. Click en **"Add New Project"**
3. Selecciona el repositorio `cotizador-creo`
4. Deja todo por defecto → click **"Deploy"**
5. En ~30 segundos tendrás una URL como: `https://cotizador-creo.vercel.app`

### 3. Dominio personalizado (opcional)

En Vercel → Settings → Domains → agrega `cotizador.creodecreerycrear.cl`
y apunta el CNAME en tu DNS a `cname.vercel-dns.com`

### 4. Incrustar en WordPress

Agrega este bloque HTML en cualquier página de tu WordPress:

```html
<iframe
  src="https://cotizador-creo.vercel.app"
  width="100%"
  height="850px"
  style="border:none; border-radius:12px;"
  title="Cotizador CREO de Creer y Crear"
  loading="lazy"
></iframe>
```

O simplemente comparte el enlace directo con tus clientes.

## Archivos

- `index.html` — toda la app (HTML + CSS + JS en un solo archivo)
- `vercel.json` — configuración de Vercel

## Actualizar precios o servicios

Abre `index.html` y edita el array `programs` o `services` en el bloque `<script>`.
Luego haz `git push` y Vercel redesplegará automáticamente.
