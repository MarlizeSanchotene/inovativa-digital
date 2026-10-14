# Inovativa Digital: site

Site estático (HTML + CSS, sem build) da Inovativa Digital, de Marlize Sanchotene.

## Estrutura

- `index.html`: página única (hero, serviços, como funciona, sobre, loja, contato)
- `style.css`: identidade visual (vinho `#9b1a31`, amarelo `#f6c21b`, creme `#f4eae6`)
- `assets/`: coloque aqui `logo.png` (sua logo oficial) quando quiser trocar a lâmpada em SVG do cabeçalho

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `inovativa-digital`).
2. Na pasta do projeto:
   ```
   git remote add origin https://github.com/SEU_USUARIO/inovativa-digital.git
   git push -u origin main
   ```
3. No GitHub: **Settings > Pages > Source: Deploy from a branch > main / (root)**.
4. O site fica em `https://SEU_USUARIO.github.io/inovativa-digital/`.

## Ligar o domínio (depois da compra)

1. Crie um arquivo chamado `CNAME` na raiz, com uma única linha: `inovativa.digital`
2. No painel de DNS do domínio:
   - 4 registros `A` para `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - 1 registro `CNAME` para `www` apontando para `SEU_USUARIO.github.io`
3. No GitHub Pages, marque **Enforce HTTPS** quando o certificado for liberado.

## Pendências para você decidir

- Logo oficial em `assets/logo.png` (hoje há uma lâmpada em SVG como substituta).
- WhatsApp comercial: o site hoje só usa e-mail e Instagram. Se quiser o botão de WhatsApp, é só informar o número.
- Mostrar ou não a associação ao Sindilojas (confirme com eles se há regra de uso da marca).
