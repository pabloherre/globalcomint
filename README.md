# GlobalComint – SEO Files

## Archivos incluidos y dónde subirlos

Todos los archivos van en la RAÍZ del repositorio (misma carpeta que `index.html`):

```
globalcomint/
├── index.html          ← tu archivo principal
├── robots.txt          ← NUEVO
├── sitemap.xml         ← NUEVO
├── site.webmanifest    ← NUEVO
└── img/
    ├── og-image.jpg    ← NUEVO (ver instrucciones abajo)
    ├── favicon-16x16.png
    ├── favicon-32x32.png
    ├── favicon-192x192.png
    ├── favicon-512x512.png
    └── apple-touch-icon.png
```

---

## Paso 1 – Pegar el snippet en index.html

Abrí `head-seo-snippet.html` y copiá TODO el contenido.
Pegalo dentro del `<head>` de tu `index.html`, reemplazando o
complementando cualquier `<meta>` que ya exista.

---

## Paso 2 – Crear la imagen OG (og-image.jpg)

Es la imagen que aparece cuando compartís el link en WhatsApp, LinkedIn, etc.
- Tamaño: **1200 × 630 px**
- Contenido sugerido: logo GlobalComint + texto "Despachantes de Aduana · Mendoza"
- Fondo oscuro (navy #0a1628) con texto en dorado (#e8b84b)
- Guardala como `img/og-image.jpg`

Podés crearla gratis en: https://canva.com

---

## Paso 3 – Crear favicons

Generá todos los tamaños desde tu logo en: https://favicon.io o https://realfavicongenerator.net

Descargá y copiá a la carpeta `img/`:
- favicon-16x16.png
- favicon-32x32.png
- favicon-192x192.png
- favicon-512x512.png
- apple-touch-icon.png (180×180)

---

## Paso 4 – Actualizar datos reales

En `head-seo-snippet.html` buscá y reemplazá:
- `+54-261-XXX-XXXX` → tu número real de teléfono
- Si tenés redes sociales, agregá las URLs en el array `"sameAs": []`

En `sitemap.xml`:
- `<lastmod>` → actualizarlo cada vez que modifiques el sitio

---

## Paso 5 – Registrar en Google Search Console

1. Entrá a https://search.google.com/search-console
2. Añadí la propiedad: `https://pabloherre.github.io/globalcomint/`
3. Verificá con el método "Etiqueta HTML" (te da un meta tag para pegar en el head)
4. Enviá el sitemap: `https://pabloherre.github.io/globalcomint/sitemap.xml`

---

## Paso 6 – Registrar en Bing Webmaster Tools

1. Entrá a https://www.bing.com/webmasters
2. Importá desde Google Search Console (tarda 1 clic)
   → Bing también indexa Yahoo automáticamente.

---

## Checklist final

- [ ] robots.txt subido a la raíz
- [ ] sitemap.xml subido a la raíz
- [ ] site.webmanifest subido a la raíz
- [ ] Snippet pegado en el <head> del index.html
- [ ] og-image.jpg creada y subida a img/
- [ ] Favicons generados y subidos a img/
- [ ] Número de teléfono real en el schema JSON-LD
- [ ] Registrado en Google Search Console + sitemap enviado
- [ ] Registrado en Bing Webmaster Tools

Con esto tu sitio estará correctamente indexado en Google, Bing, Yahoo,
DuckDuckGo, y mostrará preview enriquecido en WhatsApp, LinkedIn y Facebook.
