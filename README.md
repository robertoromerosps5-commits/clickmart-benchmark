# Clickmart · Benchmark de Marca (Julio 2026)

Reporte de benchmark competitivo de **Clickmart** (asistencia de viaje internacional, Ecuador) frente a sus 4 competidores digitales relevantes: **Assist Card**, **Universal Assistance**, **GO! Assistance** y **Seguro de Viaje Mundial**.

## Contenido del reporte

El reporte es un sitio estático interactivo (`index.html`) con:

1. **Resumen ejecutivo** — 6 hallazgos con semáforo 🔴 / 🟡 / 🟢
2. **Auditoría web comparativa** — framework, SSR vs SPA, HTML entregado, tracking, SEO on-page
3. **Presencia en Google & SEO** — indexación, sitemap, hreflang, JSON-LD
4. **Redes sociales** — seguidores por marca y matriz de presencia multicanal
5. **Meta Ads (Clickmart)** — spend, CPM, CTR, embudo, píxel y eventos disparados
6. **10 hallazgos priorizados** — con acción específica
7. **Plan 30 / 60 / 90 días**

## Stack

- HTML estático (sin build step)
- Tailwind CSS (CDN)
- Chart.js (CDN) para todos los gráficos
- Alpine.js (CDN) para tabs interactivos

## Publicar en GitHub Pages

```bash
# 1. Crear repo en GitHub (privado o público) llamado por ejemplo "clickmart-benchmark"
gh repo create clickmart-benchmark --public --source=. --push

# 2. Habilitar Pages desde la rama main /root
gh api -X POST repos/:owner/clickmart-benchmark/pages -f source[branch]=main -f source[path]=/
```

Al terminar, el reporte queda accesible en:
`https://<tu-usuario>.github.io/clickmart-benchmark/`

## Ver localmente

Simplemente abrir `index.html` en un navegador. No requiere servidor.

## Fuentes de datos

- **Meta Ads:** Meta Marketing API oficial (cuenta `act_948316490944757`), rango 2026-06-20 → 2026-07-19
- **Píxel:** Endpoint activities del pixel `4624343074460372`, últimas 24 h
- **Web:** HTML raw vía curl sobre las 5 URLs, análisis manual de meta tags, sitemap y tracking
- **Redes:** Búsqueda web + snippets públicos de perfiles
- **Google:** Consulta `site:clickmart.com.ec` en búsqueda pública

## Fecha de corte

20 de julio de 2026.

---

Reporte confidencial · Next Level Media
