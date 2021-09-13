---
title: 'user: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a3c179f2b6645b69267e1158d0f4bd2d0cf8df78
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109658"
---
# <a name="user-revokesigninsessions"></a>user: revokeSignInSessions

Namespace: microsoft.graph

Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado. Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo, exigindo que o usuário entre novamente em todos os aplicativos que eles consentiram anteriormente, independentemente do dispositivo.

>Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização inválido, o aplicativo receberá um erro. Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação ao ponto de extremidade de autorização, o que forçará o usuário a entrar.

>[!NOTE]
>Depois de **chamar revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes que os tokens sejam revogados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | User.ReadWrite.All, Directory.ReadWrite.All,|

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

Se bem-sucedido, este método retorna um código de resposta `204 No Content`.

>[!NOTE]
>Essa API tem um [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code). Ele retorna um código de resposta HTTP diferente.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
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

---


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
  ]
}
-->

