🚀 Automação de Gestão de Leads: Google Sheets + WhatsApp API Este projeto consiste em um fluxo de automação desenvolvido no N8N para otimizar o tempo de resposta do time comercial. O sistema monitora novas entradas em uma planilha de pesquisa (provenientes do Google Forms) e notifica instantaneamente o time de vendas via WhatsApp sempre que um lead demonstra interesse em contato.

📋 Problema Real Empresas perdem leads por demora no primeiro contato. Dados estagnados em planilhas dependem de verificação manual, o que gera gargalos.

💡 Solução Uma automação "real-time" que filtra interesse real de compra e/ou demonstração e entrega os dados do lead diretamente no bolso (WhatsApp) do time comercial e técnico.

🛠️ Tecnologias Utilizadas N8N: Orquestrador de automação (Cloud).

Google Sheets API: Como banco de dados e gatilho.

Z-API: Integração com a API do WhatsApp.

JSON: Para manipulação e tratamento de dados.

⚙️ Funcionalidades do Workflow Monitoramento Ativo: O nó do Google Sheets observa novas linhas na planilha.

Filtro Inteligente: Um nó de condição (If) verifica se o campo de "Desejo de Contato" foi preenchido com "Sim".

Deduplicação e Tratamento: Garantia de que a mensagem seja enviada somente ao grupo específico.

Notificação Formatada: Envio de mensagem estruturada para o grupo do WhatsApp com os dados de contato do lead (Nome, Empresa, telefone/e-mail).

👨‍💻 Autor Walter Resquin - Desenvolvedor de Automações. Localizado em: São Caetano do Sul - SP.
