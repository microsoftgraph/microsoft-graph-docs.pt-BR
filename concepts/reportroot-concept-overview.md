---
title: Visão geral da API de relatórios do Microsoft Graph
description: Os relatórios de uso do centro de administração do Microsoft 365 permitem que os administradores entendam o uso que sua empresa faz dos serviços do Office 365. Você pode usar a API de relatórios do Microsoft Graph para realizar a integração com os relatórios de uso do Office 365.
ms.openlocfilehash: d923d0003a276be15620998c53693a9bab7116d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091673"
---
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
|Microsoft Teams|[Uso do dispositivo](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>|[Atividades do usuário](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0)|
|Office 365 (geral) |[Ativações](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[Usuários ativos](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[Atividades de grupos](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0)|
|OneDrive |[Atividades](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[Uso](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0)|
|Outlook|[Atividades](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[Uso do aplicativo](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[Uso de caixa de correio](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0)|
|SharePoint |[Atividades](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[Uso do site](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0)|
|Skype for Business |[Atividades](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Atividades dos participantes](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[Atividades de ponto a ponto](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0)|
|Yammer |[Atividades](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[Atividades de grupos](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0)|

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de relatórios de uso do Office 365 no Microsoft Graph v1.0](/graph/api/resources/report?view=graph-rest-1.0)
- [API de relatórios de uso do Office 365 no Microsoft Graph beta](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
* Saiba mais sobre como [usar a API REST de relatórios](/graph/api/resources/report?view=graph-rest-1.0).
