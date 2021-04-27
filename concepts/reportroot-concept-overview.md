---
title: Visão geral da API de relatórios do Microsoft Graph
description: A API de relatórios do Microsoft Graph permite o entendimento da atividade de recursos de aplicativos e locatários.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.custom: scenarios:getting-started
ms.openlocfilehash: 52247aa125745055f4fec5b651c8c175597d1b82
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055593"
---
# <a name="microsoft-graph-reports-api-overview"></a>Visão geral da API de relatórios do Microsoft Graph

A API de relatórios do Microsoft Graph permite entender as atividades de aplicativos e recursos no seu locatário no Azure Active Directory.

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

## <a name="what-data-can-i-access-by-using-the-reports-apis"></a>Quais dados eu posso acessar usando as APIs de relatórios?

Você pode utilizar as APIs de relatórios para acessar os conjuntos de dados listados na tabela a seguir.

| APIs de relatórios | Conjunto de dados |
|:------------ |:-------- |
| Atividade | [Auditoria de diretório](/graph/api/resources/directoryaudit?view=graph-rest-1.0)<br/>[Entrar](/graph/api/resources/signin?view=graph-rest-1.0)<br/>[Provisionamento (Visualização)](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) |
| Aplicativos AD FS | [Resumo detalhado da parte de confiança (Visualização)](/graph/api/resources/relyingpartydetailedsummary?view=graph-rest-beta) |
| Registro de aplicativo | [Contagem da credencial de registro de usuário (Visualização)](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta)<br/>[Detalhes da credencial de registro de usuário (Visualização)](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) <br/>[Detalhes de utilização da credencial do usuário (Visualização)](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) <br/>[Resumo de utilização da credencial (Visualização)](/graph/api/resources/credentialusagesummary?view=graph-rest-beta)|
| Entrar no aplicativo | [Resumo da entrada (Visualização)](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) <br/>[Detalhes da entrada (Visualização)](/graph/api/resources/applicationsignindetailedsummary?view=graph-rest-beta)|
| Microsoft Teams | [Uso do dispositivo](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>[Atividades do usuário](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0) |
| Microsoft 365 (geral) | [Ativações](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[Usuários ativos](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[Atividades de grupos](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0) |
| OneDrive | [Atividades](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[Uso](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0) |
| Outlook | [Atividades](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[Uso do aplicativo](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[Uso de caixa de correio](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0) |
| SharePoint | [Atividades](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[Uso do site](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0) |
| Skype for Business | [Atividades](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Atividades dos participantes](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[Atividades de ponto a ponto](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0) |
| Yammer | [Atividades](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[Uso do dispositivo](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[Atividades de grupos](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0) |

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de relatórios de acesso e identidade do Microsoft Graph beta](/graph/api/resources/report-identity-access?view=graph-rest-beta)
- [API de relatórios de uso do Microsoft 365 no Microsoft Graph v1.0](/graph/api/resources/report?view=graph-rest-1.0)
- [API de relatórios de uso do Microsoft 365 no Microsoft Graph beta](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
* Saiba mais sobre como [usar a API REST de relatórios](/graph/api/resources/report?view=graph-rest-1.0).
