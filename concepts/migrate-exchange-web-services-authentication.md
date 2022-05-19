---
title: Diferenças de autenticação entre Exchange Web Services (EWS) e Microsoft Graph
description: Descreve os detalhes de autenticação para ajudá-lo a migrar Exchange aplicativos EWS (Serviços Web) para o Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: be933068b459aabeb0d2a7aca083b0745fa3c97a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549614"
---
# <a name="authentication-differences-between-exchange-web-services-ews-and-microsoft-graph"></a>Diferenças de autenticação entre Exchange Web Services (EWS) e Microsoft Graph

Exchange Serviços Web (EWS) e o Microsoft Graph usam plataforma de identidade da Microsoft [OAuth 2.0 para](/azure/active-directory/develop/active-directory-v2-protocols) autenticação e autorização.

> [!NOTE]
> Atualmente, o EWS também dá suporte à autenticação básica. [A autenticação básica foi preterida](/lifecycle/announcements/exchange-online-basic-auth-deprecated) e está sendo desativada em Microsoft 365 organizações. O Microsoft Graph não dá suporte à autenticação básica, portanto, os aplicativos que ainda não migraram para o OAuth 2.0 devem fazer isso para acessar o Microsoft Graph.

## <a name="permissions"></a>Permissões

O EWS e o Microsoft Graph oferecem dois tipos de permissões: delegado e aplicativo. As permissões delegadas estão no contexto de um usuário autenticado. As permissões de aplicativo são concedidas a um aplicativo que não age em nome de um usuário.

Com o EWS, um aplicativo tem acesso a tudo o que o usuário tem acesso (no caso de permissões delegadas) ou a tudo o que o EWS pode acessar (com permissões de aplicativo). 

O EWS tem um modelo de acesso todo ou nada e não há escopo granular para limitar o acesso a dados em uma caixa de correio. Enquanto que o Microsoft Graph oferece permissões granulares para recursos específicos em uma Exchange Online de correio. Por exemplo, é possível permitir que um aplicativo leia apenas mensagens de email e não tenha acesso a calendários ou contatos. As permissões efetivas para autenticação delegada são a interseção dos privilégios do usuário e as permissões que foram consentidos para o aplicativo. Para autenticação de aplicativo, as permissões efetivas são o conjunto de permissões consentidos por um administrador.

Para obter uma lista completa de Exchange microsoft Graph relacionadas, consulte:

- [Permissões de email](permissions-reference.md#mail-permissions)
- [Permissões de calendário](permissions-reference.md#calendars-permissions)
- [Permissões de contatos pessoais](permissions-reference.md#contacts-permissions)
- [Permissões de tarefas](permissions-reference.md#tasks-permissions)

## <a name="impersonation"></a>Representação

[A representação do EWS](/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange) fornece um mecanismo para que aplicativos EWS executados como uma conta de serviço atuem como um usuário. Isso permite que o aplicativo execute ações, como enviar um email, que parecem vir do usuário representado.

Com o Microsoft Graph, não há contas de serviço. Em vez disso, as permissões são concedidas diretamente aos aplicativos. O aplicativo é autenticado usando [o fluxo de credenciais do cliente](auth-v2-service.md) com sua própria identidade. Por padrão, o consentimento do administrador concede acesso às caixas de correio de todos os usuários, mas os aplicativos podem ser limitados a caixas de [correio específicas](auth-limit-mailbox-access.md) por um administrador. A maneira de obter a Representação no Microsoft Graph é usando a política de acesso a aplicativos e permissões de aplicativo.
