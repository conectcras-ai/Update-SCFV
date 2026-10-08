# Update-SCFV

Versão publicada: 1.0.40.

Autorização de exceção etária com justificativa obrigatória, ID/login/nome do usuário autenticado e data/hora do servidor. Histórico consultável em Participantes vinculados > Autorizações. Vínculo e autorização usam a mesma transação. Inclui o formulário compacto de grupo com seleção de Dia/dias da semana. Atualize primeiro o CRAS 1.0.33 e confirme a migração V2026_10_08_02, depois todos os clientes SCFV; versões antigas não geram esta auditoria. Autorizações antigas não são retroativamente atribuídas. Testes automatizados isolados passaram; validação visual e execução no MySQL ainda pendentes.

Canal: https://github.com/conectcras-ai/Update-SCFV

Arquivos: manifest.xml, public.pem e app/ConectSCFV-1.0.0-all.jar.
O manifesto é assinado e inclui versão, tamanho, checksum e assinatura do binário.
O nome físico do JAR permanece estável para as instalações existentes.
Use Sobre > Verificar / Atualizar agora. A publicação não instala automaticamente nos computadores.
