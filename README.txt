Livro Histórico v52 / App v52

Alterações desta versão:
- LDS: removido o botão redundante “Atualizar LDS”.
- LDS: mantido apenas o botão “Importar LDS”.
- LDS: o botão “Importar LDS” agora cobre primeira importação e substituição completa da base existente.
- LDS: adicionada importação com modal bloqueante de progresso percentual por etapas.
- LDS: modal exibe etapa atual, percentual e barra de progresso durante leitura/processamento/indexação.
- LDS: navegação interna fica bloqueada durante a importação para evitar inconsistência.
- LDS: importação valida o XLSX antes de apagar a base anterior, reduzindo risco de perda por arquivo inválido.

Módulo alterado:
- LDS

Módulos preservados:
- Launcher/tela inicial
- Livro Histórico
- Livro Histórico DA
- Horas
- Relatórios
- Dashboard
- Notas / Bloco de notas
- Backup
- PDFs
- Topbar
- Navegação geral

Observações técnicas:
- A busca LDS, os cards e o compartilhamento LDS foram preservados.
- A estrutura IndexedDB foi mantida.
- O progresso é calculado por fases e por lotes durante a gravação, evitando atualização de DOM a cada registro.
- A versão visual do app/menu foi atualizada para v52.

Histórico recente:
- v48: módulo LDS offline com IndexedDB e busca corrigida.
- v49: Bloco de Notas com altura automática, sem rolagem interna na nota, botão expandir/recolher e persistência individual.
- v50: LDS com botão Compartilhar em cada card de resultado.
- v51: LDS com compartilhamento refinado nos cards.
- v52: LDS com importação única e modal de progresso bloqueante.
