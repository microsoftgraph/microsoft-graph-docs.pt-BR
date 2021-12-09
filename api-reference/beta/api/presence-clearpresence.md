---
title: 'presença: clearPresence'
description: Desmarcar as informações de presença para a sessão de presença do aplicativo do usuário.
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: af78f3718c45861b82428c6733c1dc8e7468bfc0
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390875"
---
# <a name="presence-clearpresence"></a>presença: clearPresence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Desmarcar uma sessão de](presence-setpresence.md#presence-sessions) presença de um aplicativo para um usuário. Se for a única sessão de presença do usuário, uma **clearPresence** bem-sucedida altera a presença do usuário para `Offline/Offline` .

Leia mais sobre [sessões de presença](presence-setpresence.md#presence-sessions) e seu [tempo de expiração e expiração.](presence-setpresence.md#timeout-expiration-and-keep-alive) 

## <a name="permissions"></a>Permissões
A permissão a seguir é necessária para chamar a API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Presence.ReadWrite                          |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo   | Descrição                                   |
| :-------- | :----- | :-------------------------------------------- |
| sessionId | string | A ID da sessão de presença do aplicativo. |


> [!IMPORTANT]
> 
> Forneça a ID do aplicativo como `sessionId` na solicitação.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `200 OK`.

Se a sessão de presença não existir, este método retornará um `404 NotFound` código de resposta.

## <a name="examples"></a>Exemplos
A solicitação a seguir mostra o aplicativo com ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que limpa sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clear--presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clear--presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clear--presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clear--presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clear--presence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
