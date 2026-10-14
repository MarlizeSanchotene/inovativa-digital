# Inovativa Digital: site

Site estático (HTML + CSS, sem build) da Inovativa Digital, de Marlize Sanchotene.

## Estrutura

- `index.html`: página única (hero, serviços, como funciona, sobre, loja, contato)
- `style.css`: identidade visual (vinho `#9b1a31`, amarelo `#f6c21b`, creme `#f4eae6`)
- `assets/logo.jpg`: logo oficial (174x187 px, baixa resolução; troque por uma versão maior do Canva mantendo o nome do arquivo, ou ajuste o nome no `index.html`)

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

1. Crie um arquivo chamado `CNAME` na raiz, com uma única linha: `inovativa.app`
2. No painel de DNS do domínio:
   - 4 registros `A` para `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - 1 registro `CNAME` para `www` apontando para `SEU_USUARIO.github.io`
3. No GitHub Pages, marque **Enforce HTTPS** quando o certificado for liberado.

## Domínio escolhido: inovativa.app

- O `.app` só funciona com HTTPS. O GitHub Pages já entrega HTTPS, então sem problema.
- Na compra, confira no checkout: o que está incluído no "gratuito por 1 ano", o valor da renovação e se há condição (como exigir um plano). Ative a renovação automática e crie um lembrete de calendário 60 dias antes do vencimento.
- No Wix, o DNS é editado em **Domínios > (seu domínio) > Gerenciar registros DNS**. Siga os registros da seção anterior.

## Loja virtual (Nuvemshop)

- O link antigo da bio (`/melhores-ofertas`) dá 404. Troque o link da bio do Instagram pela raiz da loja assim que ela abrir.
- O site mostra "Loja virtual em breve". Quando a loja estiver no ar, siga o comentário dentro da seção `loja` do `index.html` e coloque o link real.

## Pendências para você decidir

- Logo em alta resolução (hoje há 174x187 px).
- WhatsApp comercial: o site hoje só usa e-mail e Instagram. Se quiser o botão de WhatsApp, é só informar o número.
- Mostrar ou não a associação ao Sindilojas (confirme com eles se há regra de uso da marca).
