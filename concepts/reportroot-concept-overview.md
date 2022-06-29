---
title: Visão geral da API de relatórios do Microsoft Graph
description: Você pode usar a API de relatórios para incorporar os dados de uso do Microsoft 365 à solução de relatórios existente na sua organização, para que todos os relatórios do serviço de TI estejam em um único local.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
ms.custom: scenarios:getting-started
ms.openlocfilehash: 84718f4a6fb1b0046387e6338980c99e5d91b881
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446123"
---
# <a name="microsoft-graph-reports-api-overview"></a>Visão geral da API de relatórios do Microsoft Graph

A API de relatórios do Microsoft Graph permite entender as atividades de aplicativos e recursos no seu locatário no Azure Active Directory (Azure AD).

> [!VIDEO https://www.youtube-nocookie.com/embed/P6HneRXYdx8]

## <a name="why-use-the-reports-api"></a>Por que usar a API de relatórios?

### <a name="integrate-microsoft-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Integre os relatórios de uso do Microsoft 365 à solução de relatórios existente na sua organização
Muitas empresas têm soluções de relatório existentes que utilizam um aplicativo ou o portal da Web para gerar relatórios. Você pode usar a API de relatórios para incorporar os dados de uso do Microsoft 365 à solução de relatórios existente na sua organização, para que todos os relatórios do serviço de TI estejam em um único local.

### <a name="retain-usage-reports-for-historical-analysis"></a>Reter relatórios de uso para análise de histórico
Você pode usar a API de relatórios para obter os dados que estão disponíveis nos relatórios de uso, incluindo resumos no nível da organização de acordo com o serviço, informações de uso no nível da entidade (usuários, sites, contas) dos últimos 7/30/90/180 dias e agregações de atividades diárias. Isso lhe dá a opção de manter informações históricas de uso pelo tempo que for necessário.

### <a name="analyze-ad-fs-application-activity-and-configuration"></a>Analise a atividade e configuração do aplicativo AD FS
Fornece informações sobre uma terceira parte confiável configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração da terceira parte confiável pode ser migrada para o Azure Active Directory.

### <a name="monitor-application-sign-ins"></a>Monitorar logins de aplicativos

Monitore o uso dos seus aplicativos e tome decisões sobre os padrões de uso.

### <a name="determine-who-is-using-your-applications-and-how-are-they-using-them"></a>Defina quem está usando seus aplicativos e como eles os estão usando

Os relatórios de uso dos métodos de autenticação ajudam a entender como os usuários da sua organização utilizam os recursos do Azure Active Directory (Azure AD), como descanso de senha de autoatendimento e autenticação multifatorial (MFA). Esses relatórios ajudam a determinar quais métodos de autenticação são mais bem-sucedidos para sua organização, quais tipos de erros os usuários finais estão enfrentando e qual a campanha que você precisa executar para ajudar seus usuários finais a adotar o uso de descanso por senha de autoatendimento e MFA.

### <a name="monitor-activity-on-an-azure-ad-tenant"></a>Monitorar a atividade em um locatário do Microsoft Azure Active Directory

Entenda melhor como seus usuários acessam e utilizam os serviços do Microsoft Azure Active Directory. Você pode analisar os dados para criar soluções personalizadas adaptadas às necessidades específicas da sua organização.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>Quais dados eu posso acessar usando a API de relatórios?

Você pode usar a API de relatórios para acessar os conjuntos de dados listados na tabela a seguir.

| APIs de relatórios | Conjunto de dados |
|:------------ |:-------- |
| Atividade | [Auditoria de diretório](/graph/api/resources/directoryaudit)<br/>[Entrar](/graph/api/resources/signin)<br/>[Provisioning](/graph/api/resources/provisioningobjectsummary) |
| Aplicativos AD FS | [Resumo detalhado da parte de confiança (visualização)](/graph/api/resources/relyingpartydetailedsummary) |
| Registro de aplicativo | [Contagem da credencial de registro de usuário (visualização)](/graph/api/resources/credentialuserregistrationcount)<br/>[Detalhes da credencial de registro de usuário (visualização)](/graph/api/resources/credentialuserregistrationdetails) <br/>[Detalhes de utilização da credencial do usuário (visualização)](/graph/api/resources/usercredentialusagedetails) <br/>[Resumo de utilização da credencial (visualização)](/graph/api/resources/credentialusagesummary)|
| Entrar no aplicativo | [Resumo da entrada (visualização)](/graph/api/resources/applicationsigninsummary) <br/>[Detalhes da entrada (visualização)](/graph/api/resources/applicationsignindetailedsummary)|
| Microsoft Teams | [Uso do dispositivo](/graph/api/resources/microsoft-teams-device-usage-reports)<br/>[Uso da equipe](/graph/api/resources/microsoft-teams-team-usage-reports)<br/>[Atividades do usuário](/graph/api/resources/microsoft-teams-user-activity-reports)|
| Microsoft 365 (geral) | [Ativações](/graph/api/resources/office-365-activations-reports)<br/>[Usuários ativos](/graph/api/resources/office-365-active-users-reports)<br/>[Atividades de grupos](/graph/api/resources/office-365-groups-activity-reports) |
| OneDrive | [Atividades](/graph/api/resources/onedrive-activity-reports)<br/>[Uso](/graph/api/resources/onedrive-usage-reports) |
| Outlook | [Atividades](/graph/api/resources/email-activity-reports)<br/>[Uso do aplicativo](/graph/api/resources/email-app-usage-reports)<br/>[Uso de caixa de correio](/graph/api/resources/mailbox-usage-reports) |
| SharePoint | [Atividades](/graph/api/resources/sharepoint-activity-reports)<br/>[Uso do site](/graph/api/resources/sharepoint-site-usage-reports) |
| Skype for Business | [Atividades](/graph/api/resources/skype-for-business-activity-reports)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[Atividades dos participantes](/graph/api/resources/skype-for-business-participant-activity-reports)<br/>[Atividades de ponto a ponto](/graph/api/resources/skype-for-business-peer-to-peer-activity) |
| Yammer | [Atividades](/graph/api/resources/yammer-activity-reports)<br/>[Uso do dispositivo](/graph/api/resources/yammer-device-usage-reports)<br/>[Atividades de grupos](/graph/api/resources/yammer-groups-activity-reports) |

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de relatórios de identidade e acesso no Microsoft Graph beta](/graph/api/resources/report-identity-access?view=graph-rest-beta&preserve-view=true)
- [API de relatórios de uso do Microsoft 365 no Microsoft Graph v1.0](/graph/api/resources/report?view=graph-rest-1.0&preserve-view=true)
- [API de relatórios de uso do Microsoft 365 no Microsoft Graph beta](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Próximas etapas

* Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
