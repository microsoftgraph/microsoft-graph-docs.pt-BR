---
title: Visão geral sobre o API do log de auditoria AD Azure
description: Azure Active Directory (AD Azure) rastreia métricas de atividade e a entrada do usuário e auditoria de cria relatórios de log que ajudarão-lo a entender como os usuários acessam e aproveitem os serviços do Azure AD. Use a API do Microsoft Graph para Azure AD para analisar os dados base esses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.
ms.openlocfilehash: b25e9820d4f6df0c6a38fc9784a37ce8a82ceeb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034590"
---
# <a name="azure-ad-audit-log-api-overview"></a>Visão geral sobre o API do log de auditoria AD Azure

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Azure Active Directory (AD Azure) rastreia métricas de atividade e a entrada do usuário e auditoria de cria relatórios de log que ajudarão-lo a entender como os usuários acessam e aproveitem os serviços do Azure AD. Use a API do Microsoft Graph para Azure AD para analisar os dados base esses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.

## <a name="what-are-azure-ad-activity-logs"></a>Cite atividade do Azure AD logs?

Azure AD fornece dois tipos de logs de atividade:

- logs de auditoria 
- logs de entrar

### <a name="audit-logs"></a>Logs de auditoria

O relatório de atividade de logs de auditoria oferece acesso ao histórico de cada tarefa seja executada no seu locatário. O relatório de logs de auditoria fornece registros de atividades do sistema para fins de conformidade. Entre outros, os dados fornecidos permite abordar cenários comuns, como:

- Quem concedida acesso de administração de grupo a um usuário de diretório?

- Quais usuários estão entrando para um aplicativo adquirido recentemente?

- Redefine as senhas quantos foram feitos dentro do diretório?

### <a name="sign-in-logs"></a>Inscreva-se nos logs

O relatório de atividade de logons ajuda a determinar quem executou as tarefas relatadas pelo relatórios do log de auditoria. O relatório de atividade de logons ajuda você a responder perguntas como:

- O que é o padrão de um usuário entrar?
- Quantos usuários tem entrado durante a última semana?
- Qual é o status dessas entradas?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>O que pode fazer com que o log de auditoria APIs no Microsoft Graph?

Aqui estão as solicitações de populares para trabalhar com dados de log de auditoria:

Operação | URL
:----------|:----
Obtenha as atividades do usuário de Inquilino | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
OBTER locatário entradas do usuário | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>Quais licenças são necessárias?

Relatórios do log de auditoria estão disponíveis para os recursos que você licenciou.  Se você tiver uma licença para um recurso específico, você também tem acesso aos seus logs de auditoria.

Por exemplo, você precisa de uma licença do Windows Azure AD Premium P1 para acessar os relatórios de auditoria de senha de autoatendimento.  Para saber mais, consulte [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Relatórios de entrar exigem uma licença do Windows Azure AD Premium.

Para saber mais, consulte [preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Próximas etapas

- [Registrar seu aplicativo](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender a pré-requisitos de log de auditoria. 
- Saiba do [log de auditoria](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) e [exemplos de entrada](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Revise o recurso [directoryAudit](directoryaudit.md) e ações.
- Revise o recurso de [logon](signin.md) e ações. 