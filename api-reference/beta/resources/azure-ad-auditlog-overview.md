---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b8b53037c70ff68523f51dd266da69518a1cc57a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133040"
---
# <a name="activity-reports-api-overview"></a>Visão geral da API de relatórios de atividades

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD. Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.

A disponibilidade desses relatórios de atividades é regida pelas políticas de retenção de dados do Microsoft Azure Active Directory. Para saber mais, confira [políticas de retenção de dados](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="what-are-activity-reports"></a>O que são relatórios de atividades?

O Microsoft Azure Active Directory fornece três tipos de relatórios de atividades:

- Auditorias de diretório 
- Entradas
- Provisionamento

### <a name="directory-audits"></a>Auditorias de diretório

O relatório de auditoria de diretório fornece acesso ao histórico de todas as tarefas executadas em seu locatário. O relatório de auditoria de diretório fornece registros de atividades do sistema para conformidade. Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:

- Quem concedeu acesso ao grupo de administradores a um usuário de diretório?
- Quais usuários estão se conectando a um aplicativo adquirido recentemente?
- Quantas redefinições de senhas foram feitas no diretório?

### <a name="sign-ins"></a>Entradas

O relatório de entradas ajuda a determinar quem executou as tarefas relatadas pelas auditorias de diretório. O relatório de entrada ajuda você a responder a perguntas como:

- O que é o padrão de entrada de um usuário?
- Quantos usuários entraram durante a semana passada?
- Qual é o status dessas entradas?

### <a name="provisioning"></a>Provisionamento

O relatório de aprovisionamento ajuda a ver todas as ações executadas pelo serviço de provisionamento do Microsoft Azure Active Directory. O relatório de aprovisionamento ajuda a responder a perguntas como:

- Quais grupos foram criados com sucesso no ServiceNow?
- Quais funções foram importadas dos serviços Web da Amazon?
- Quais usuários foram criados sem sucesso a partir da workday?

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a>O que posso fazer com os relatórios de atividades do Microsoft Graph?

Aqui estão solicitações populares para trabalhar com dados de relatório:

Operation | URL
:----------|:----
OBTER atividades de usuário do locatário | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
OBTER entradas de usuário do locatário | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
OBTER logs de provisionamento | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

Os relatórios de atividades estão disponíveis para os recursos que você licenciou. Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.

Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.  Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Relatórios de entrada requerem uma licença do Azure AD Premium.

Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Próximas etapas

- [Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório. 
- Aprenda com [amostras do log de auditoria](/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Analisar recurso e ações do [directoryAudit](directoryaudit.md).
- Analisar recurso e ações do [signIn](signin.md). 
- Analisar o recurso[provisioningObjectSummary](provisioningobjectsummary.md).
