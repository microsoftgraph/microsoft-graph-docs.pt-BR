---
title: Trabalhar com relatórios de uso do Microsoft 365 no Microsoft Graph
description: Com o Microsoft Graph, você pode acessar recursos de relatórios de uso do Microsoft 365 para obter informações sobre como as pessoas em sua empresa estão usando os serviços Microsoft 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Microsoft 365.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 937f1c18efe074a0fdec3dc02b31f393dd6ca40c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855621"
---
# <a name="working-with-microsoft-365-usage-reports-in-microsoft-graph"></a>Trabalhar com relatórios de uso do Microsoft 365 no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Com o Microsoft Graph, você pode acessar recursos de relatórios de uso do Microsoft 365 para obter informações sobre como as pessoas em sua empresa estão usando os serviços do Microsoft 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Microsoft 365. 

Para obter detalhes sobre as configurações que regem a identificação/des identificação de informações nos dados Microsoft 365 relatórios de uso, consulte [Relatórios do Microsoft 365 no centro de administração](/microsoft-365/admin/activity-reports/activity-reports).

## <a name="authorization"></a>Autorização

O Microsoft Graph controla o acesso a recursos por meio de permissões. Você deve especificar as permissões necessárias para acessar os recursos dos Relatórios. Normalmente, você deve especificar permissões no portal do Azure Active Directory (Azure AD). Para saber mais, veja [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e[Permissões de relatórios](/graph/permissions-reference#reports-permissions).

## <a name="settings"></a>Settings

Nos relatórios do Microsoft 365, as informações do usuário, como nomes de usuário, grupos e sites, são ocultadas; os valores reais não são exibidos. Você pode usar a API [adminReportSettings ](../resources/adminreportsettings.md) para controlar a exibição de informações do usuário nos relatórios.

## <a name="cloud-deployments"></a>Implantações na nuvem

A tabela a seguir mostra a disponibilidade de cada API em todas as implantações na nuvem.

| APIs                                                         | Serviço global do Microsoft Graph | **Microsoft Cloud para o Governo dos EUA** | **Microsoft Cloud China operado pela 21Vianet** | **Microsoft Cloud Germany** |
| ------------------------------------------------------------ | ------------------------------ | ------------------------------------- | ---------------------------------------------- | --------------------------- |
| [Ativações do Microsoft 365](/graph/api/resources/office-365-activations-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Usuários ativos do Microsoft 365](/graph/api/resources/office-365-active-users-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Uso de aplicativos do Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Uso do navegador Microsoft 365](/graph/api/resources/microsoft-365-browser-usage-report?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Atividade de grupos do Microsoft 365](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Uso do dispositivo do Microsoft Teams](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Uso do Microsoft Teams pela equipe](/graph/api/resources/microsoft-teams-team-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Atividade de usuários do Microsoft Teams](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Atividade do Outlook](/graph/api/resources/email-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Uso do aplicativo do Outlook](/graph/api/resources/email-app-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Uso de caixas de correio do Outlook](/graph/api/resources/mailbox-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Atividade do OneDrive](/graph/api/resources/onedrive-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Uso do OneDrive](/graph/api/resources/onedrive-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Atividade do SharePoint](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Uso do site do SharePoint](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Atividade do Skype for Business](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Uso do dispositivo do Skype for Business](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Atividade do organizador do Skype for Business](/graph/api/resources/skype-for-business-organizer-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Atividade de participantes do Skype for Business](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Atividade de colega para colega do Skype for Business](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Atividade do Yammer](/graph/api/resources/yammer-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Uso do dispositivo do Yammer](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Atividade de grupos do Yammer](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

APIs e recursos de relatório podem criar novas maneiras de se relacionar com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).


