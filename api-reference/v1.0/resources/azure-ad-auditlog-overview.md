---
title: Visão geral da API de log de auditoria do Azure AD
description: O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e usam os serviços do Azure AD.
localization_priority: Priority
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 7c91aea96c93065a469b64bb3088540928e2e1d3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033072"
---
# <a name="azure-ad-audit-log-api-overview"></a>Visão geral da API de log de auditoria do Azure AD

O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e usam os serviços do Azure AD. Use a API do Microsoft Graph para o Azure AD para analisar os dados desses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.

## <a name="what-are-azure-ad-activity-logs"></a>O que são logs de atividade do Azure AD?

O Azure AD oferece dois tipos de logs de atividade:

- Logs de auditoria
- Logs de entrada

### <a name="audit-logs"></a>Logs de auditoria

O relatório de atividades de logs de auditoria fornece acesso ao histórico de todas as tarefas executada em seu locatário. O relatório de logs de auditoria fornece registros de atividades do sistema de conformidade. Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:

- Quem concedeu acesso ao grupo de administradores a um usuário de diretório?
- Quais usuários estão se conectando a um aplicativo adquirido recentemente?
- Quantas redefinições de senhas foram feitas no diretório?

### <a name="sign-in-logs"></a>Logs de entrada

O relatório de atividade de entrada ajuda a determinar quem realizou as tarefas relatadas pelos relatórios de log de auditoria. O relatório de atividades de entrada ajuda a responder perguntas como:

- O que é o padrão de entrada de um usuário?
- Quantos usuários entraram durante a semana passada?
- Qual é o status dessas entradas?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de log de auditoria no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER atividades de usuário do locatário | [OBTER https://graph.microsoft.com/v1.0/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
OBTER entradas de usuário do locatário | [OBTER https://graph.microsoft.com/v1.0/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

Os relatórios de log de auditoria estão disponíveis para os recursos que você tiver licenciado.  Se você tiver uma licença para um recurso específico, também terá acesso a seus logs de auditoria.

Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.  Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Relatórios de entrada requerem uma licença do Azure AD Premium.

Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Próximas etapas

- [Registre seu aplicativo](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para satisfazer aos pré-requisitos do log de auditoria. 
- Aprenda com [amostras do log de auditoria](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Analisar recurso e ações do [directoryAudit](directoryaudit.md).
- Analisar recurso e ações do [signIn](signin.md). 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
