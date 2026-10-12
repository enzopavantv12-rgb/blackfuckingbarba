# FuckingBarba — Pré-Black 2026

Projeto estático pronto para GitHub e Vercel. Prévia 09, com 36 roteiros,
editor de textos, avaliações, referências de vídeo, criativos e cenários.

## Enviar ao GitHub

1. Extraia o ZIP.
2. Abra o repositório desejado e selecione **Add file → Upload files**.
3. Envie o conteúdo extraído: a pasta `public`, `vercel.json`, `README.md`
   e `.gitignore`. Preserve a estrutura de pastas.
4. Confirme o envio com **Commit changes**.

Envie os arquivos extraídos, não o ZIP. Se o repositório já contiver outro
site, mantenha este projeto numa pasta própria e selecione essa pasta como
Root Directory na Vercel. Não substitua arquivos de outro projeto.

## Conectar à Vercel

1. Acesse https://vercel.com/new e conecte sua conta do GitHub.
2. Autorize o acesso ao repositório desejado e clique em **Import**.
3. Configure:

| Campo | Valor |
| --- | --- |
| Framework Preset | Other |
| Root Directory | Pasta com o `vercel.json`; raiz se estes arquivos estiverem na raiz |
| Build Command | Vazio; não há etapa de build |
| Output Directory | public |
| Install Command | Nenhum comando necessário |

4. Clique em **Deploy** e aguarde a URL do projeto.

O `vercel.json` já define a pasta `public` e dispensa build.
Atualizações enviadas à branch de produção conectada geram nova publicação.

## Edições e avaliações

Os textos-base ficam no HTML. Alterações feitas pelo editor e avaliações
são salvas somente no navegador da pessoa. Não são enviadas ao GitHub,
à Vercel ou a outros usuários. Para transferir suas edições locais para o
site publicado, exporte a revisão na página atual e importe o JSON no site.
Não há banco de dados compartilhado nesta versão.

## Organização

- `public/index.html`: página principal com roteiro-base e interface.
- `public/assets/`: imagens, fonte e prévias de vídeo separadas.
- `public/*.zip`: pacotes de imagens para download na página.
- `public/*.md`: documentos de apoio.
- `vercel.json`: configuração de hospedagem.

As mídias foram separadas para reduzir o HTML e facilitar o envio ao GitHub.
O conteúdo do projeto e suas funções de edição foram preservados.

Documentação oficial consultada:
- https://vercel.com/docs/git
- https://vercel.com/docs/builds/configure-a-build
- https://vercel.com/docs/project-configuration/vercel-json
- https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
