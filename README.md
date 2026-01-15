# ⚡ Minhas Automações n8n

Bem-vindo ao meu repositório de workflows para [n8n](https://n8n.io/). Este projeto reúne automações desenvolvidas para integrar diferentes serviços, processar dados e eliminar tarefas repetitivas.

## 📂 O que tem aqui?

Aqui você encontrará arquivos `.json` que podem ser importados diretamente para o seu editor n8n. As automações cobrem casos de uso como:

* **Integração de APIs:** Conexão entre [Serviço A] e [Serviço B].
* **Processamento de Dados:** Tratamento e formatação de JSONs complexos.
* **Automação de Notificações:** Envios automáticos via Slack/Email/Telegram.
* **Triggers Personalizados:** Workflows acionados via chamadas HTTP do front-end.

## 🚀 Workflows Destaque

| Workflow | Descrição | Trigger |
| :--- | :--- | :--- |
| `Sync_Lead_CRM.json` | Sincroniza novos leads do front-end para o CRM | Webhook/HTTP |
| `Daily_Report.json` | Gera relatório diário e envia por e-mail | Cron (Schedule) |
| `Data_Sanitization.json` | Limpeza e padronização de dados de entrada | Manual/Execute |

## Pré-requisitos

Para rodar estes workflows, você precisará de:

* Uma instância do n8n (Self-hosted ou Cloud) versão `1.x` ou superior.
* As credenciais configuradas para os serviços utilizados (ex: Chave de API do OpenAI, Google Sheets, etc.).

## Como usar

1.  **Clone o repositório** ou baixe o arquivo `.json` desejado:
    ```bash
    git clone [https://github.com/seu-usuario/seu-repo-n8n.git](https://github.com/seu-usuario/seu-repo-n8n.git)
    ```
2.  **No n8n:**
    * Crie um novo workflow.
    * Clique no menu (três pontos no canto superior direito) > **Import from File**.
    * Selecione o arquivo `.json`.
3.  **Configuração:**
    * Revise os nós de credenciais (eles aparecerão com aviso se faltar a conexão).
    * Ative o workflow.

## Segurança e Credenciais

As credenciais **NÃO** estão incluídas nos arquivos JSON deste repositório por motivos de segurança.
* Certifique-se de configurar suas próprias credenciais no n8n.
* Se estiver usando variáveis de ambiente, verifique o nó `Set` ou as configurações globais.

## Contribuição

Sugestões e melhorias são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.
