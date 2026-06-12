# votumhub-site

Site institucional da Votum, servido via GitHub Pages no domínio
**votumhub.com**. Estático, sem build — editar os `.html` direto e dar push.

## Estrutura

- `index.html` — página única (hero, serviços, método, contato)
- `privacidade.html` — Política de Privacidade (LGPD; também é pré-requisito do
  app review da Meta)
- `termos.html` — Termos de Uso
- `CNAME` — domínio custom do GitHub Pages

## DNS (uma vez, no provedor do domínio)

Apontar `votumhub.com` para o GitHub Pages:

| Tipo | Nome | Valor |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | jhonatasmenezes.github.io |

Depois, em Settings → Pages do repositório, confirmar o custom domain
`votumhub.com` e marcar **Enforce HTTPS** (o certificado é emitido
automaticamente em alguns minutos após o DNS propagar).

## Pendências de conteúdo

- Rodapé: incluir razão social + CNPJ (consistência com o Business Manager da
  Meta e o Google Business).
- Criar o e-mail `contato@votumhub.com` (alias) ou trocar o endereço nos HTML.
- Preencher os meta tags de verificação comentados no `<head>` do `index.html`
  (Google Search Console e Meta Business) quando gerar os códigos.
