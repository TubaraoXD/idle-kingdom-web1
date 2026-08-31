# Como colocar isso num link pra testar no celular

Esses arquivos (`index.html`, `index.wasm`, etc.) são o jogo já "compilado" pra rodar
direto no navegador. Só falta colocar num servidor. Aqui vão 2 caminhos:

## Opção rápida (testar agora, sem criar conta)

1. Acesse **https://app.netlify.com/drop**
2. Arraste esta pasta inteira pra lá.
3. Em alguns segundos você recebe um link público (tipo `nome-aleatorio.netlify.app`).
4. Abre esse link no navegador do celular.

## Opção permanente com GitHub + Vercel (pra eu conseguir atualizar depois)

1. Crie um repositório novo no GitHub (ex: `idle-kingdom-web`).
2. Suba esta pasta pra dentro dele.
3. Vá em **https://vercel.com**, conecte esse repositório, Deploy (configuração padrão,
   é HTML estático).
4. Me manda um token do GitHub (fine-grained, com permissão só nesse repositório)
   quando quiser que eu suba uma atualização direto.

## Detalhe técnico

Build exportado **sem threads**, de propósito — funciona em qualquer servidor simples
(Netlify, Vercel, GitHub Pages, itch.io) sem precisar configurar cabeçalhos especiais.
