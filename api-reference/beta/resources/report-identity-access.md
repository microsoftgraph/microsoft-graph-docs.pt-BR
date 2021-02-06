---
title: Visão geral da API de relatórios de identidade e acesso
description: Acesse a identidade e os relatórios de acesso para obter informações sobre como as pessoas da sua empresa estão usando os aplicativos no locatário do Azure Active Directory.
localization_priority: Priority
ms.prod: identity-and-access-reports
author: besiler
doc_type: conceptualPageType
ms.openlocfilehash: 567bfdfd848c2a7f1df19b8aad76a68774a6bf0e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129363"
---
# <a name="identity-and-access-reports-api-overview"></a>Visão geral da API de relatórios de identidade e acesso

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Com o Microsoft Graph, você pode usar a identidade de acesso e os relatórios de acesso para obter informações sobre como as pessoas da sua empresa estão usando aplicativos no locatário do Azure Active Directory (Azure AD).

## <a name="authorization"></a>Autorização

O Microsoft Graph controla o acesso aos recursos utilizando permissões. Você deve especificar as permissões necessárias para acessar os recursos dos relatórios. Para saber mais, veja [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e[Permissões de relatórios](/graph/permissions-reference#reports-permissions).

## <a name="what-are-identity-and-access-reports"></a>O que são relatórios de identidade e acesso?

Os seguintes relatórios de identidade e acesso estão disponíveis para ajudá-lo a entender a atividade do aplicativo no seu locatário:

- Atividade de aplicativo no AD FS
- Entrar no aplicativo
- Registro e utilização

### <a name="ad-fs-application-activity"></a>Atividade de aplicativo no AD FS

O relatório de atividades do aplicativo AD FS fornece informações sobre como uma terceira parte confiável é configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração da terceira parte confiável pode ser migrada para o Azure Active Directory. Para obter mais informações, consulte o recurso [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

### <a name="application-sign-in"></a>Entrar no aplicativo

Avalie o uso de logins de aplicativos no seu locatário utilizando um relatório de resumo ou um relatório que forneça detalhes de entradas, como o número de entradas e se ocorreu algum erro durante a entrada. Para mais informações, consulte o recurso [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

### <a name="registration-and-usage"></a>Registro e utilização

Entenda melhor como os usuários da sua organização utilizam os recursos do Microsoft Azure Active Directory, como o autoatendimento para redefinição de senha e autenticação multifatorial (MFA). Você pode determinar quais métodos de autenticação são mais bem-sucedidos para sua organização, quais tipos de erros os usuários finais estão enfrentando e qual campanha você precisa executar para ajudar seus usuários finais a adotar o uso do autoatendimento para redefinição de senha e MFA. Para obter mais informações, consulte a [API de relatório de uso de métodos de autenticação](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

## <a name="next-steps"></a>Próximas etapas

APIs e recursos de relatório podem criar novas maneiras para você relacionar-se com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).


