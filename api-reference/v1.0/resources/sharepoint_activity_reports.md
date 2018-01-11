# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot_getsharepointactivityuserdetail.md) | Fluxo      | Obtenha dados sobre as atividades do SharePoint por usuário. |
| [Obter contagens de arquivo](../api/reportroot_getsharepointactivityfilecounts.md) | Fluxo      | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot_getsharepointactivityusercounts.md) | Fluxo      | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot_getsharepointactivitypages.md) | Fluxo      | Obtenha o número de páginas exclusivas visitadas pelos usuários. |
