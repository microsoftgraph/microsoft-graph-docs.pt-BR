---
title: 'usuário: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ab60a38e404dc13dbbc58b1103931cfe0b16c44
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083946"
---
# <a name="user-revokesigninsessions"></a>usuário: revokeSignInSessions

Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado. Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo solicitando que o usuário entre novamente em todos os aplicativos para os quais tenham sido consentidos anteriormente, independentemente do dispositivo.

>Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro. Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.

>[!NOTE]
>Após chamar o **revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes de os tokens serem revogados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | User. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Directory.ReadWrite.All, Directory.AccessAsUser.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Esta operação não tem conteúdo de solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```

##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
