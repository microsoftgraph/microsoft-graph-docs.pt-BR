---
title: 'user: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos e cookies de sessão no navegador do usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a13982cb924c5c9b82c3248aefc13a54ec44bb2e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351045"
---
# <a name="user-invalidateallrefreshtokens"></a>user: invalidateAllRefreshTokens

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data-hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.  Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo sem que o usuário seja obrigado a entrar novamente. Na verdade, essa operação forçaria o usuário a entrar novamente em todos os aplicativos que eles consentiram anteriormente, independentemente do dispositivo.

Para desenvolvedores, se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização inválido, o aplicativo receberá um erro. Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação ao ponto de extremidade de autorização, o que forçará o usuário a entrar.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

+ Para que um aplicativo permita que o usuário inscreve invalide os aplicativos aos qual ele consentiu: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All
+ Para um aplicativo permitir que um administrador invalide aplicativos que um usuário consentiu: Directory.ReadWrite.All, Directory.AccessAsUser.All

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Esta operação não tem conteúdo de solicitação.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `204 No Content`.

>[!NOTE]
>Essa API retorna um código de resposta HTTP diferente, semelhante à ação [revokeSignInSessions.](user-revokesigninsessions.md) Para obter detalhes, consulte [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code). 

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


