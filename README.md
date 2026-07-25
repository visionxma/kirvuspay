# KIRVUSPAY — Landing Page

Landing page institucional da **KIRVUSPAY**, gateway de pagamentos com Pix, cartão e criptomoedas.

Site estático, **100% offline** (sem dependências externas: fontes, ícones, scripts e imagens são todos locais em `_ext/`).

## Estrutura

- `index.html` — página principal
- `_ext/` — assets (imagens, fontes Oxanium/Manrope, ícones, logos, OG image)
- `robots.txt`, `sitemap.xml`, `site.webmanifest` — arquivos de SEO/PWA

## SEO

- Meta tags, Open Graph e Twitter Cards completos
- Dados estruturados JSON-LD (Organization, WebSite, WebPage, Service, FAQPage)
- Imagem OG dedicada (`_ext/og-image.jpg`, 1200×630)
- `sitemap.xml` + `robots.txt`

## Rodar localmente

```bash
python3 -m http.server 8765
# abra http://127.0.0.1:8765
```

## Deploy

Basta servir os arquivos estáticos (GitHub Pages, Vercel, Netlify, etc.).
> Domínio de referência nas meta tags: `https://kirvuspay.com.br` — ajuste se publicar em outro domínio.
