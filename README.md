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
   git remote add origin https://github.com/MarlizeSanchotene/inovativa-digital.git
   git push -u origin main
   ```
3. No GitHub: **Settings > Pages > Source: Deploy from a branch > main / (root)**.
4. O site fica em `https://MarlizeSanchotene.github.io/inovativa-digital/`.

## Ligar o domínio inovativa.digital (Hostinger)

1. O arquivo `CNAME` já está na raiz do projeto, com `inovativa.digital`.
2. Recomendado: verifique o domínio no GitHub antes (no seu perfil: **Settings > Pages > Add a domain**). Ele pede um registro `TXT`, que você cria no mesmo painel de DNS do passo 3. Isso evita que outra pessoa se passe pelo seu domínio.
3. Na Hostinger: **Domínios > inovativa.digital > Gerenciar > DNS / Servidores de nomes > Registros DNS**.
   - Apague os registros `A` e `AAAA` do `@` e o `CNAME` do `www` que já existirem (são da página de estacionamento).
   - Crie 4 registros `A` para `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Crie 1 registro `CNAME` para `www` apontando para `MarlizeSanchotene.github.io` (sem o nome do repositório).
   - Deixe os servidores de nomes da própria Hostinger. Se estiverem apontando para outro lugar, os registros acima não valem.
4. No GitHub: **Settings > Pages > Custom domain: inovativa.digital > Save**. Quando o certificado for liberado (pode levar de minutos a algumas horas), marque **Enforce HTTPS**.
5. Renovação: na Hostinger, ative a renovação automática e anote a data de vencimento. Crie um lembrete de calendário 60 dias antes.

## Loja virtual (Nuvemshop)

- O link antigo da bio (`/melhores-ofertas`) dá 404. Troque o link da bio do Instagram pela raiz da loja assim que ela abrir.
- O site mostra "Loja virtual em breve". Quando a loja estiver no ar, siga o comentário dentro da seção `loja` do `index.html` e coloque o link real.

## Pendências para você decidir

- Logo em alta resolução (hoje há 174x187 px).
- WhatsApp comercial: o site hoje só usa e-mail e Instagram. Se quiser o botão de WhatsApp, é só informar o número.
- Mostrar ou não a associação ao Sindilojas (confirme com eles se há regra de uso da marca).

## Link do formulário de briefing

O botão do topo, o destaque da página inicial e a seção de contato apontam para o Google Formulário. Para trocar o link, procure no `index.html` por `docs.google.com/forms` (3 ocorrências) e substitua.
