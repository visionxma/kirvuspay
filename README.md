# KIRVUSPAY — Landing Page

Landing page institucional da **KIRVUSPAY**, gateway de pagamentos com Pix, cartão e criptomoedas.

Site estático, **100% offline** (sem dependências externas: fontes, ícones, scripts e imagens são todos locais em `_ext/`).

## Estrutura

```
.
├── index.html              # página principal
├── robots.txt              # SEO
├── sitemap.xml             # SEO
├── site.webmanifest        # PWA
└── _ext/                   # assets (todos locais)
    ├── fonts/              # fontes (Oxanium, Manrope) .woff2
    ├── img/                # imagens (webp/jpg/svg)
    ├── icons/              # logos, favicon, ícones do app
    ├── docs/               # PDFs (termos de uso)
    └── vendor/             # scripts de terceiros
```

> Pastas `_backups/` e `_dev/` são locais (ferramentas/backups) e não vão pra produção (ver `.gitignore`).

## SEO

- Meta tags, Open Graph e Twitter Cards completos
- Dados estruturados JSON-LD (Organization, WebSite, WebPage, Service, FAQPage)
- Imagem OG dedicada (`_ext/img/og-image.jpg`, 1200×630)
- `sitemap.xml` + `robots.txt`

## Rodar localmente

```bash
python3 -m http.server 8765
# abra http://127.0.0.1:8765
```

## Deploy

Basta servir os arquivos estáticos (Cloudflare Pages, GitHub Pages, Vercel, Netlify, etc.).
> Domínio de referência nas meta tags: `https://kirvuspay.com.br` — ajuste se publicar em outro domínio.
