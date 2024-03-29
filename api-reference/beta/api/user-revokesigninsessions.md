---
title: 'user: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 50cbd3a7b85817b2591ad927fae91549a1a0a55f
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671885"
---
# <a name="user-revokesigninsessions"></a>user: revokeSignInSessions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado. Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo, exigindo que o usuário entre novamente em todos os aplicativos que eles consentiram anteriormente, independentemente do dispositivo.

Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização inválido, o aplicativo receberá um erro. Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação ao ponto de extremidade de autorização, o que forçará o usuário a entrar.

>[!NOTE]
>Depois de **chamar revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes que os tokens sejam revogados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | User.ReadWrite.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | User.ReadWrite.All, Directory.ReadWrite.All |

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
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
Esta operação não tem conteúdo de solicitação.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`.

>[!NOTE]
>Essa API tem um [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-http-code). Ele retorna um código de resposta HTTP diferente.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "ignored",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-revokesigninsessionss-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-revokesigninsessionss-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.Boolean",
    "value": true
}
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
  ]
}
-->


