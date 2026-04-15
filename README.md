# Fazenda Canoa — WordPress Block Theme

> Block theme oficial da Landing Page **Reserva Fazenda Canoa** — estrutura pronta para deploy via **Deployer for Git**, WP-CLI ou upload manual. Os arquivos do tema estão no **root** deste repositório (padrão WordPress).

**Site:** [lago.fazendacanoa.com.br](https://lago.fazendacanoa.com.br)
**Autor:** [RUCH](https://ruch.digital)
**Repositório principal (com protótipo e docs):** [lago-fazenda-canoa](https://github.com/rafaelruch/lago-fazenda-canoa)
**Plugin dependente:** [lfc-opcoes-plugin](https://github.com/rafaelruch/lfc-opcoes-plugin)

---

## 🚀 Deploy via Deployer for Git

1. No admin WordPress → **Deployer for Git** → Adicionar
2. **URL do repositório:** `https://github.com/rafaelruch/fazenda-canoa-theme.git`
3. **Pasta destino:** `wp-content/themes/fazenda-canoa`
4. **Branch:** `main`
5. Salvar e executar o deploy

Depois:
- **Aparência → Temas** → ativar **"Fazenda Canoa"**
- **Plugins** → ativar **"Fazenda Canoa — Opções & Leads"** (do repo [lfc-opcoes-plugin](https://github.com/rafaelruch/lfc-opcoes-plugin))
- **Configurações → Fazenda Canoa** → revisar contatos

## 📁 Estrutura

```
(root do repo) = tema fazenda-canoa
├── style.css            # Declaração do tema
├── theme.json           # Design tokens
├── functions.php
├── index.php
├── screenshot.png
├── README.md            # Este arquivo
├── MANUAL-EDICAO.md     # Manual pro time comercial
├── inc/                 # SEO + Performance
│   ├── seo.php          # Structured Data + meta tags + GSC/GA4/Pixel
│   └── performance.php  # Preload LCP + cleanup WP bloat + security headers
├── templates/           # front-page, index, landing-page
├── parts/               # header, footer, floating-widget
├── patterns/            # 9 block patterns editáveis
└── assets/
    ├── css/main.css
    ├── js/main.js
    ├── fotos/           # 37 fotos otimizadas (17MB total)
    └── logos/           # 7 logos + favicon
```

## ✨ Features

- **Block theme 100% nativo** (FSE) — editável via Site Editor do WP
- **9 block patterns** (1 por seção) — edição livre de conteúdo
- **Template parts** com placeholders dinâmicos resolvidos via filter `render_block`
- **Structured Data (Schema.org JSON-LD)** — WebSite, Organization, RealEstateListing, Place, BreadcrumbList, FAQPage
- **Meta tags SEO completas** + Open Graph + Twitter Cards + Geo tags
- **Performance** — preload LCP, dns-prefetch, JS deferred, lazy loading
- **Cleanup WordPress bloat** — emoji scripts, generator, RSS, oembed, wlwmanifest, XML-RPC
- **Security headers** — X-Content-Type-Options, X-Frame-Options, Referrer-Policy, Permissions-Policy
- **Integrações Google/Meta** — campos para GSC verification, GA4 ID, Meta Pixel ID (via plugin `lfc-opcoes`)
- **Admin bar compatibility** — nav não some atrás da barra do WP quando logado
- **Imagens otimizadas** — 539MB→17MB (97% redução, max 1600px, quality 82)

## 🔧 Dependências

- WordPress **6.5+**
- PHP **7.4+**
- Plugin [`lfc-opcoes`](https://github.com/rafaelruch/lfc-opcoes-plugin) (contatos globais + CPT Leads + webhook)

## 🎨 Design tokens principais

| Token | Valor |
|---|---|
| `paper` | `#FFFFFF` |
| `ink` | `#1A1A1A` |
| `accent` | `#1F7A3F` (verde natureza) |
| `warning` | `#B8710F` (corten) |
| `whatsapp` | `#25D366` |
| Tipografia | **Manrope** 300–700 |
| Container | 1180px |

## 📝 Licença

GPL-2.0-or-later

---

Desenvolvido por [RUCH](https://ruch.digital).
