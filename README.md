README - Portfolio com GSAP (versão pronta para deploy)

Arquivos incluídos:
- index.html
- styles.css
- script.js (com GSAP/ScrollTrigger integrados via CDN)
- assets/ (placeholders: logo.png, avatar.jpg, project*-*.jpg, favicon.png)

O que foi adicionado:
- GSAP + ScrollTrigger para animações scroll-driven (reveal de seções, parallax na hero, animações do modal e cards).
- Tudo integrado via CDN — NÃO é necessário instalar node/npm. Abra index.html e teste localmente no navegador.
- Código comentado no script.js para facilitar edições (velocidades, desativar efeitos, etc).

Como testar localmente:
1. Extraia o ZIP em uma pasta.
2. Abra o arquivo index.html no navegador (Chrome / Firefox). Algumas funcionalidades do ScrollTrigger funcionam melhor se servido via HTTP (por exemplo, usando `npx http-server`), mas normalmente funcionam abrindo o arquivo localmente.

Deploy rápido no Vercel (opção recomendada — atualizações automáticas via GitHub)
A) Criar repositório no GitHub:
  1. Crie uma conta em github.com (ou entre na sua conta).
  2. Crie um novo repositório (ex: fabricio-portfolio).
  3. Faça commit e push dos arquivos (index.html, styles.css, script.js, assets/).

B) Conectar no Vercel (importar do GitHub):
  1. Acesse vercel.com e crie uma conta (ou entre).
  2. Clique em 'New Project' > 'Import Git Repository' > selecione o repositório que você criou.
  3. Aceite permissões (o Vercel pede acesso ao repo).
  4. Em 'Build settings' geralmente não precisa alterar nada — é um site estático. Clique em 'Deploy'.
  5. O Vercel irá gerar uma URL tipo `your-repo.vercel.app`. Para produção, configure domínio personalizado se desejar.

Opção rápida (arrastar e soltar):
  1. No dashboard do Vercel clique em 'New Project' > 'Import Project' > 'Upload' (drag & drop).
  2. Selecione a pasta que contém index.html (ou o ZIP). O Vercel publicará automaticamente.

Opção CLI (terminal):
  1. Instale Vercel CLI: `npm i -g vercel` (é necessário ter Node instalado).
  2. No terminal, navegue até a pasta do site e rode `vercel` e siga as instruções interativas.
  3. Quando estiver pronto para produção rode `vercel --prod`.

Observações e dicas de edição:
- Para editar a velocidade do parallax/entradas: abrir `script.js` e ajustar valores em `gsap.to` / `gsap.from` (comentários indicam onde alterar).
- Para adicionar ou remover animações: procure por `initGSAP()` e os blocos dentro dele; você pode comentar ou ajustar facilmente.
- Manter as imagens nos arquivos `assets/` e usar os nomes sugeridos facilita atualizar sem mexer no HTML.

Se quiser, eu posso também:
- Criar o repositório no GitHub com esses arquivos (posso te fornecer um ZIP pronto — já incluído) e te mandar o passo-a-passo com prints detalhados de cada clique no Vercel (com imagens). Como eu não tenho acesso às suas contas, você fará os cliques finais — eu guio passo-a-passo.
- Integrar funcionalidades adicionais (Lightbox com thumbnails, galeria filtrável, ou botão de download do PDF do portfólio).

Boa parte técnica está pronta — quer que eu gere o ZIP para download agora?
