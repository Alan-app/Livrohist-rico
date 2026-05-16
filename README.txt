Livro Histórico v50 / App V04

Correções desta versão:

BUG 1 — Modal de conflito ao importar backup ultrapassando a linha amarela da topbar
- Modal agora se inicia abaixo da topbar fixa usando padding-top baseado em --topbar-height.
- Altura máxima limitada a calc(100vh - topbar - margens), com overflow-y:auto interno.
- Nenhuma outra lógica, botão ou estilo do modal foi alterado.

BUG 2 — Modal de imagem dos lançamentos cortando topbar e ficando grande demais
- Modal de visualização de imagem agora respeita totalmente a área útil abaixo da topbar.
- Imagem usa object-fit:contain e max-height calculado via viewport menos topbar e margens.
- SwipeArea usa flex:1 para ocupar espaço disponível sem transbordar para cima ou para baixo.
- Proporção original da imagem preservada. Zoom/pinça não alterado.

BUG 3 — Voltar após editar lançamento indo para tela errada
- Após salvar edição de lançamento, o app agora navega automaticamente para Ver Histórico.
- O fluxo correto foi restaurado: Ver Histórico → Editar → Salvar → Ver Histórico.
- Comportamento do botão Voltar e demais telas não foi alterado.


Versão v48: módulo LDS offline com IndexedDB.

Versão v49: Bloco de Notas com altura automática, sem rolagem interna na nota, botão expandir/recolher e persistência individual do estado.


Versão v50: LDS com botão Compartilhar em cada card de resultado.
- Módulo alterado: LDS, exclusivamente nos cards de resultado da busca.
- Funcionalidade adicionada: compartilhamento dos dados completos do card via Web Share API quando disponível.
- Fallback implementado para WhatsApp Web/App usando https://wa.me/?text= com encodeURIComponent.
- Dados compartilhados: Functional Mark, Parent Functional Mark, Long LCN Nomenclature, Equipment Description, ICC, NSN, TM Number, Allow on board e Allow ShoreBase.
- Importação XLSX, IndexedDB, índices e lógica de busca LDS preservados.
- Demais módulos preservados: Launcher, Livro Histórico, Livro Histórico DA, Horas, Relatórios, Dashboard, Notas, Backup, PDFs, topbar e navegação geral.


Versão v51: LDS com compartilhamento refinado nos cards.
- Módulo alterado: LDS, exclusivamente no botão de compartilhar e no texto compartilhado.
- Botão grande com texto removido dos cards LDS.
- Novo botão usa ícone SVG inline local, pequeno, discreto, sem dependência online, com title e aria-label “Compartilhar”.
- Texto compartilhado formatado para WhatsApp com título em negrito, campos separados por linhas em branco e valores vazios como “-”.
- Web Share API preservada quando disponível e fallback WhatsApp via https://wa.me/?text= preservado.
- Importação XLSX, IndexedDB, índices e lógica de busca LDS preservados.
- Demais módulos preservados: Launcher, Livro Histórico, Livro Histórico DA, Horas, Relatórios, Dashboard, Notas, Backup, PDFs, topbar e navegação geral.
