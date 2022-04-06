---
title: Diferenças de autenticação entre Exchange Web Services (EWS) e Microsoft Graph
description: Descreve detalhes de autenticação para ajudá-lo a migrar aplicativos Exchange Web Services (EWS) para o Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 120efa7e2fc4c34b973831131d8fb2c435c2c432
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516543"
---
# <a name="authentication-differences-between-exchange-web-services-ews-and-microsoft-graph"></a>Diferenças de autenticação entre Exchange Web Services (EWS) e Microsoft Graph

Exchange Web Services (EWS) e o Microsoft Graph usam o [plataforma de identidade da Microsoft OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols) para autenticação e autorização.

> [!NOTE]
> Atualmente, o EWS também oferece suporte à autenticação básica. [A autenticação básica é preterida](/lifecycle/announcements/exchange-online-basic-auth-deprecated) e está sendo desativada em Microsoft 365 organizações. O Microsoft Graph não dá suporte à autenticação básica, portanto, os aplicativos que ainda não migraram para o OAuth 2.0 devem fazer isso para acessar o Microsoft Graph.

## <a name="permissions"></a>Permissões

O EWS e o Microsoft Graph oferecem dois tipos de permissões: delegado e aplicativo. As permissões delegadas estão no contexto de um usuário autenticado. Permissões de aplicativo são concedidas a um aplicativo que não age em nome de um usuário.

Com o EWS, um aplicativo tem acesso a tudo o que o usuário tem acesso (no caso de permissões delegadas) ou a tudo o que o EWS pode acessar (com permissões de aplicativo).

O Microsoft Graph oferece permissões granulares para recursos específicos em uma caixa de Exchange Online de correio. Por exemplo, é possível permitir que um aplicativo leia apenas mensagens de email e não tenha acesso a calendários ou contatos. As permissões efetivas para autenticação delegada são a interseção dos privilégios do usuário e as permissões que foram consentida para o aplicativo. Para autenticação de aplicativos, as permissões efetivas são o conjunto de permissões consentido por um administrador.

Para ver uma lista completa das Exchange do Microsoft Graph relacionadas, consulte:

- [Permissões de email](permissions-reference.md#mail-permissions)
- [Permissões de calendário](permissions-reference.md#calendars-permissions)
- [Permissões de contatos pessoais](permissions-reference.md#contacts-permissions)
- [Permissões de tarefas](permissions-reference.md#tasks-permissions)

## <a name="impersonation"></a>Representação

[A representação do EWS](/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange) fornece um mecanismo para os aplicativos EWS que são executados como uma conta de serviço para atuarem como usuários. Isso permite que o aplicativo tome ações, como o envio de um email, que parecem vir do usuário personificado.

Com o Microsoft Graph, não há contas de serviço. Em vez disso, as permissões são concedidas diretamente aos aplicativos. O aplicativo autentica usando o fluxo [de credenciais do cliente](auth-v2-service.md) com sua própria identidade. Por padrão, o consentimento do administrador concede acesso a todas as caixas de correio de usuários, mas os aplicativos podem ser limitados a caixas de [correio específicas](auth-limit-mailbox-access.md) por um administrador.
