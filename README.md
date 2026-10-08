# Update-SCFV

Publique o conteudo desta pasta no repositorio:

https://github.com/conectcras-ai/Update-SCFV

Estrutura esperada:

- manifest.xml
- app/ConectSCFV-1.0.0-all.jar

Para o botao Sobre > Atualizar sistema detectar nova versao, a versao do manifest precisa ser maior que a versao instalada.

Versao publicada: 1.0.37.

Nesta versão: removidos os botões Atualizar internos, mantendo o geral do topo;
QR Code com apenas o Fechar do rodapé; avisos específicos de CPF/NIS duplicado.
Sem nova migração de banco. 39 testes automatizados passaram sem falhas.

Novo Cadastro: responsável identificado pelo ID central, vínculo e origem
detalhada persistidos; cadastro central e inscrição salvos em uma única transação.
Inclui correções de busca de participantes e validação do cadastro.

Requisito: atualizar primeiro o ConectCRAS servidor para 1.0.31, após backup
verificado, e confirmar a migração V2026_10_07_01 nos logs do servidor.
O SCFV é cliente e não executa migrações no banco central.

Verificação: 34 testes automatizados passaram sem falhas.
