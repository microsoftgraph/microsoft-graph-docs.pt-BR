---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: a1971825f126307417002b83f013c85c6b7014dd582c5df67b6e059d2c8a04bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178602"
---
# <a name="activity-reports-api-overview"></a>Visão geral da API de relatórios de atividades

Namespace: microsoft.graph

O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD. Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.

A disponibilidade desses relatórios de atividades é regida pelas políticas de retenção de dados do Microsoft Azure Active Directory. Para saber mais, confira [políticas de retenção de dados](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="what-are-azure-ad-activity-logs"></a>O que são logs de atividade do Azure Active Directory?

O Microsoft Azure Active Directory fornece os seguintes tipos de relatórios de atividades:

- Auditorias de diretório
- Entradas

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

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de log de auditoria no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER atividades de usuário do locatário | [OBTER https://graph.microsoft.com/v1.0/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
OBTER entradas de usuário do locatário | [OBTER https://graph.microsoft.com/v1.0/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

Os relatórios de atividades estão disponíveis para os recursos que você licenciou. Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.

Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.  Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Relatórios de entrada requerem uma licença do Azure AD Premium.

Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Próximas etapas

- [Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório. 
- Para saber como recuperar os logs de auditoria enquanto são autenticados usando certificados, consulte o [Tutorial: Obter dados usando a API de relatórios do Azure Active Directory com certificados](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).   
- Analisar recurso e ações do [directoryAudit](directoryaudit.md).
- Analisar recurso e ações do [signIn](signin.md). 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
