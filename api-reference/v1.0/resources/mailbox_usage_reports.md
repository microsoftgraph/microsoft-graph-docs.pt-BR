# <a name="mailbox-usage-reports"></a>Relatórios de uso da caixa de correio

Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio]((https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de caixa de correio](../api/reportroot_getmailboxusagedetail.md) | Fluxo      | Obtenha dados sobre o uso da caixa de correio.         |
| [Obter contagens de caixa de correio](../api/reportroot_getmailboxusagemailboxcounts.md) | Fluxo      | Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email. |
| [Obter contagens da cota de status da caixa de correio](../api/reportroot_getmailboxusagequotastatusmailboxcounts.md) | Fluxo      | Obtenha a contagem de caixas de correio de usuário em cada categoria de cota. |
| [Obter armazenamento](../api/reportroot_getmailboxusagestorage.md) | Fluxo      | Obtenha a quantidade de armazenamento usada em sua organização. |
