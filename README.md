# votumhub-site

Site institucional da Votum, servido via GitHub Pages no domínio
**votumhub.com**. Estático, sem build — editar os `.html` e dar push.

Construído com a **identidade visual Votum v1.5-web** (extensão oficial da
paleta v1.4 via WF-16: Space Grotesk + DM Sans, rampa obsidian, acento ember
≤10%; tokens completos em `brand/tokens-v1.5-web.json`).

## Estrutura

- `index.html` — página única (hero com imagem oficial, serviços, método, contato)
- `privacidade.html` — Política de Privacidade (LGPD; também é pré-requisito do
  app review da Meta)
- `termos.html` — Termos de Uso
- `assets/` — wordmark oficial (`wordmark-light.svg`), `favicon.svg`, `hero.jpg`
  (gerada via media-gen, certificada contra a identidade)
- `brand/tokens-v1.5-web.json` — design tokens da identidade web
- `CNAME` — domínio custom do GitHub Pages

## DNS (uma vez, no provedor do domínio)

| Tipo | Nome | Valor |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | jhonatasmenezes.github.io |

Depois, em Settings → Pages, confirmar o custom domain `votumhub.com` e marcar
**Enforce HTTPS** (certificado automático após o DNS propagar).

## Pendências de conteúdo

- Rodapé: incluir razão social + CNPJ (consistência com Meta Business Manager e
  Google Business).
- Criar o e-mail `contato@votumhub.com` (alias) ou trocar o endereço nos HTML.
- Preencher as meta tags de verificação comentadas no `<head>` do `index.html`
  (Google Search Console e Meta Business) quando gerar os códigos.
