# SCFV 1.0.46

## Agenda e desempenho

- Semana atual por padrão; Hoje/Semana/Mês/Personalizado.
- Grupo, situação e busca por atividade, grupo ou educador.
- Consulta paginada no banco: 25/50/100 sessões; ordenação por data, hora e ID.
- Calendário mensal carrega apenas totais por dia; clicar em um dia abre a lista paginada.
- Mantém a geração antecipada recorrente e a prevenção de duplicidade existentes.

## Sessões e presença

- Iniciar: apenas PROGRAMADA e na data da sessão, conforme o banco.
- Finalizar: apenas EM_ANDAMENTO e na data da sessão.
- Não realização: selecione uma ou várias sessões PROGRAMADAS (até 100 por operação),
  escolha FERIADO/RECESSO/OUTRO MOTIVO e informe justificativa.
- Para recesso, use período personalizado e selecione as sessões desejadas na página.
- A operação é transacional. Preserva os registros; armazena CANCELADA para manter
  compatibilidade com os indicadores existentes que excluem sessões não realizadas.
- O motivo, a data da sessão, o login/ID e o timestamp do banco ficam nas observações;
  sessões iniciadas/encerradas não podem ser sobrescritas pelo formulário de atividade.
- Não permite cancelar sessões com presença já lançada. Não corrige automaticamente
  inconsistências históricas; elas exigem revisão da equipe.
- Presença/chegada/saída exigem sessão em andamento na data correta. Saída exige chegada
  e não pode ser repetida. Não foi criado fluxo de lançamento retroativo.
- Início, criação de lista e mudança de status são atômicos.

## Visualização e informações

- Lista de presença maior, colunas com largura mínima, rolagem horizontal e tooltip do nome.
- Entrada/Saída também tem larguras mínimas e rolagem horizontal.
- Encaminhamento interno vem da chegada e é lido pela lista de presença.
- Engajamento é informado na saída, de 1 a 5. Agora pode ficar não avaliado (NULL),
  sem assumir nota 1 automaticamente. Não altera avaliações já registradas.

Base: SISTEMAS SUAS.pdf, páginas 21 e 22 e conversa anexada de treinamento.
Não modifica dados de produção, não cria migração e não amplia acesso entre serviços.
Calendário/lista também foram renderizados e inspecionados fora da tela em 1320x850,
com dados fictícios isolados e sem iniciar a aplicação instalada. Recomenda-se conferir
o layout no monitor real após instalar. Os testes de escrita usam banco isolado.
