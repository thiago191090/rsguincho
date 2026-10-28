# RS Guincho – Landing page (GitHub Pages)

## 1. Antes de publicar: troque os dados (Ctrl+H em todos os arquivos)

| Procure | Troque por |
|---|---|
| `61900000000` | Número com DDD, só dígitos (ex.: 61999999999) |
| `(61) 90000-0000` | Número formatado para exibição |
| `+55-61-90000-0000` | Número no formato internacional (dados estruturados) |
| `rsguincho.com.br` | Domínio comprado (index.html, robots.txt, sitemap.xml, CNAME) |
| `AW-XXXXXXXXXX` e `ROTULO_...` | ID e rótulos de conversão do Google Ads (final do index.html) |

Revise também a lista de cidades em "Onde atendemos" (HTML e JSON-LD no topo) e os serviços, para bater com o que o cliente realmente faz.

## 2. Publicar
1. Crie um repositório no GitHub e envie todos os arquivos desta pasta para a raiz (inclusive `.nojekyll` e `CNAME`).
2. Settings → Pages → Source: branch `main`, pasta `/ (root)`.
3. No registro.br, aponte o domínio:
   - `www` → CNAME para `SEU-USUARIO.github.io`
   - domínio raiz (apex) → registros A: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
4. Em Settings → Pages, marque **Enforce HTTPS** quando liberar.

## 3. Depois de no ar
- Google Search Console: adicione o domínio e envie `https://www.rsguincho.com.br/sitemap.xml`.
- Teste em https://search.google.com/test/rich-results (FAQ e empresa local).
- Teste em https://pagespeed.web.dev.

## Arquivos
- `index.html` – página (CSS e JS embutidos, sem fontes externas)
- `404.html`, `robots.txt`, `sitemap.xml`, `site.webmanifest`, `CNAME`, `.nojekyll`
- `img/` – logo e foto do guincho em WebP, ícones e imagem de compartilhamento (og-image.jpg)
