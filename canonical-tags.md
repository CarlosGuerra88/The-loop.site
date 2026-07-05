# Canonical tags — pega esta línea en el `<head>` de cada archivo

Va justo después de la `<meta name="description">` de cada página.

| Archivo | Línea a pegar |
|---|---|
| `index.html` | `<link rel="canonical" href="https://the-loop.site/index.html" />` |
| `industrias.html` | `<link rel="canonical" href="https://the-loop.site/industrias.html" />` |
| `industria-ecommerce.html` | `<link rel="canonical" href="https://the-loop.site/industria-ecommerce.html" />` |
| `industria-inmobiliaria.html` | `<link rel="canonical" href="https://the-loop.site/industria-inmobiliaria.html" />` |
| `industria-gastronomia.html` | `<link rel="canonical" href="https://the-loop.site/industria-gastronomia.html" />` |
| `industria-gimnasios.html` | `<link rel="canonical" href="https://the-loop.site/industria-gimnasios.html" />` |
| `industria-dentistas.html` | `<link rel="canonical" href="https://the-loop.site/industria-dentistas.html" />` |
| `industria-retail.html` | `<link rel="canonical" href="https://the-loop.site/industria-retail.html" />` |
| `industria-automotriz.html` | `<link rel="canonical" href="https://the-loop.site/industria-automotriz.html" />` |
| `industria-coaches.html` | `<link rel="canonical" href="https://the-loop.site/industria-coaches.html" />` |
| `servicio-ads.html` | `<link rel="canonical" href="https://the-loop.site/servicio-ads.html" />` |
| `servicio-auditoria.html` | `<link rel="canonical" href="https://the-loop.site/servicio-auditoria.html" />` |
| `servicio-automatizacion.html` | `<link rel="canonical" href="https://the-loop.site/servicio-automatizacion.html" />` |
| `servicio-dashboard.html` | `<link rel="canonical" href="https://the-loop.site/servicio-dashboard.html" />` |
| `web.html` | `<link rel="canonical" href="https://the-loop.site/web.html" />` |

## Páginas de funnel (no las indexamos, no llevan canonical estándar — llevan `noindex`)

Agrega esta línea en el `<head>` de estas 3 páginas en vez de canonical:

```html
<meta name="robots" content="noindex, follow" />
```

- `gracias.html`
- `upsell.html`
- `TheLoop-diagnostico-web-sales.html`

**Por qué:** son pasos de funnel post-conversión, no destinos de búsqueda. Si Google las indexa, un prospecto puede aterrizar directo en la página de "gracias" o en el upsell sin pasar por el diagnóstico — y además ensucia el conteo de eventos del Pixel (Lead / InitiateCheckout) si el tráfico orgánico dispara esos eventos sin haber completado el paso anterior.
