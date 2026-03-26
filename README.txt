Publicação com instalação obrigatória

Arquivos:
- index.html -> página de instalação obrigatória
- app.html -> aplicativo real
- manifest.webmanifest
- service-worker.js

Comportamento:
- abrindo pelo navegador: mostra só a página "Instalar aplicativo"
- abrindo já instalado como PWA: entra direto no app

Para publicar:
1. apague os arquivos antigos do repositório
2. envie estes arquivos novos
3. aguarde o GitHub Pages atualizar
4. se o app antigo já estiver instalado, remova e instale de novo
5. se o navegador insistir em cache antigo, abra em aba anônima
