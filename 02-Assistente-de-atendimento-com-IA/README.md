🤖 Assistente de Atendimento com IA para uma serralheria
Este projeto apresenta uma solução de Atendimento Automatizado e Inteligente via WhatsApp, desenvolvida no n8n. O assistente utiliza Inteligência Artificial para qualificar leads e responder dúvidas frequentes de clientes para uma serralheria, garantindo atendimento 24/7 com uma linguagem humanizada.

📋 Cenário de Negócio
Profissionais de serviços como os de uma Serralheria, muitas vezes perdem orçamentos por estarem ocupados com o trabalho manual (solda, cortes, instalações) e por não conseguirem responder o WhatsApp instantaneamente. Esta automação atua como uma secretária virtual técnica.

💡 Diferenciais Técnicos
Baixa Latência: Uso do modelo Llama (via Groq API), permitindo respostas em milissegundos.

Filtro Anti-Spam/Grupos: Inteligência de fluxo para evitar que o robô responda em grupos, newsletters ou mensagens de broadcast, evitando responder sem necessidade e economizando tokens.

Persistência de Dados: Registro automático de todos os interessados em uma planilha para posterior acompanhamento (follow-up) comercial.

🛠️ Tecnologias Utilizadas
n8n: Plataforma de orquestração.

Z-API: Integração para recebimento e envio de mensagens via WhatsApp.

Groq API (Llama 3): Motor de IA de alta performance.

Google Sheets API: Registro de leads.

🏗️ Estrutura do Workflow
Webhook (Trigger): Recebe o payload da Z-API a cada nova mensagem.

Filtro de Mensagem:

Verifica se a mensagem é proveniente de um grupo, broadcast ou newsletter.

Registro de Lead: Extrai o senderName e senderNumber e insere em uma linha no Google Sheets.

Agente de IA (AI Agent Node):

Modelo: Llama 3 via Groq.

Prompt de Sistema: Define a persona do assistente (ajudante de uma oficina de serralheria, especialista em portões, grades e estruturas metálicas, localizada em São Caetano do Sul).

Resposta Automática: O texto gerado pela IA é enviado de volta ao cliente via POST para a Z-API.

🧠 O "Cérebro" do Assistente (System Prompt)
O agente foi configurado com um prompt que instrui a:

Identificar o tipo de serviço (Solda, Portão, Grade, etc.).

Solicitar fotos ou medidas para facilitar o orçamento.

Manter um tom profissional, porém acessível e prático.

👨‍💻 Autor
Walter Resquin - Desenvolvedor de Automações.
