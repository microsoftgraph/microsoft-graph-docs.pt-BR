# <a name="microsoft-graph-reports-api-overview"></a>Visão geral da API de relatórios do Microsoft Graph

Os relatórios de uso do centro de administração do Microsoft 365 permitem que os administradores entendam o uso que sua empresa faz dos serviços do Office 365. Você pode usar a API de relatórios do Microsoft Graph para realizar a integração com os relatórios de uso do Office 365.

## <a name="why-use-the-reports-api"></a>Por que usar a API de relatórios?

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Integrar os relatórios de uso do Office 365 com a solução de relatórios existente da sua organização
Muitas empresas têm soluções de relatório existentes que utilizam um aplicativo ou portal da Web para gerar relatórios. Você pode usar a API de relatórios para incorporar dados de uso do Office 365 na solução de relatórios existente da sua organização para que todos os relatórios de serviços de TI estejam em um local unificado.  

### <a name="retain-usage-reports-for-historical-analysis"></a>Reter relatórios de uso para análise de histórico
Você pode usar a API de relatórios para obter os dados que estão disponíveis em todos os relatórios de uso, incluindo resumos no nível da organização de acordo com o serviço, informações de uso no nível da entidade (usuários, sites, contas) para os últimos 7/30/90/180 dias e agregações de atividades diárias. Isso permite que você mantenha informações de uso históricas por quanto tempo precisar.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>Quais dados eu posso acessar usando a API de relatórios?

Você pode usar a API de relatórios para acessar os conjuntos de dados listados na tabela a seguir.

|Aplicativo do Office 365|Conjunto de dados|
|:--------|:--------|
|Microsoft Teams|[Uso do dispositivo](../api-reference/v1.0/resources/microsoft_teams_device_usage_reports.md)<br/>|[Atividades do usuário](../api-reference/v1.0/resources/microsoft_teams_user_activity_reports.md)|
|Office 365 (geral) |[Ativações](../api-reference/v1.0/resources/office_365_activations_reports.md)<br/>[Usuários ativos](../api-reference/v1.0/resources/office_365_active_users_reports.md)<br/>[Atividades de grupos](../api-reference/v1.0/resources/office_365_groups_activity_reports.md)|
|OneDrive |[Atividades](../api-reference/v1.0/resources/onedrive_activity_reports.md)<br/>[Uso](../api-reference/v1.0/resources/onedrive_usage_reports.md)|
|Outlook|[Atividades](../api-reference/v1.0/resources/email_activity_reports.md)<br/>[Uso do aplicativo](../api-reference/v1.0/resources/email_app_usage_reports.md)<br/>[Uso de caixa de correio](../api-reference/v1.0/resources/mailbox_usage_reports.md)|
|SharePoint |[Atividades](../api-reference/v1.0/resources/sharepoint_activity_reports.md)<br/>[Uso do site](../api-reference/v1.0/resources/sharepoint_site_usage_reports.md)|
|Skype for Business |[Atividades](../api-reference/v1.0/resources/skype_for_business_activity_reports.md)<br/>[Uso do dispositivo](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Uso do dispositivo](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Atividades dos participantes](../api-reference/v1.0/resources/skype_for_business_participant_activity_reports.md)<br/>[Atividades de ponto a ponto](../api-reference/v1.0/resources/skype_for_business_peer_to_peer_activity.md)|
|Yammer |[Atividades](../api-reference/v1.0/resources/yammer_activity_reports.md)<br/>[Uso do dispositivo](../api-reference/v1.0/resources/yammer_device_usage_reports.md)<br/>[Atividades de grupos](../api-reference/v1.0/resources/yammer_groups_activity_reports.md)|

## <a name="next-steps"></a>Próximas etapas

* Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer).
* Saiba mais sobre como [usar a API REST de relatórios](../api-reference/v1.0/resources/report.md).
