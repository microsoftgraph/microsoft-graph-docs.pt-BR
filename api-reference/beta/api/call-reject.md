---
title: 'Call: rejeitar'
description: Rejeite as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0134b03e27deeaf24eba3deb9c58b56865ab72d8
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792277"
---
# <a name="call-reject"></a>Call: rejeitar

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permite que o bot rejeite uma [chamada](../resources/call.md)de entrada. A solicitação de chamada de entrada pode ser um convite para uma reunião ou uma chamada ponto a ponto. A solicitação de chamada de entrada expira após 15 segundos. Se nenhuma resposta for enviada durante esse tempo, a chamada será rejeitada automaticamente.

Depois que o bot é registrado com uma URL de retorno de chamada válida no portal do Azure, a chamada de entrada é `changeType` entregue como `created`um [commsNotification](../resources/commsnotification.md) com a definição para. O bot é esperado `Answer` ou `Reject` a chamada antes que ele expire.

> **Observação:** Essa API é usada apenas para rejeitar chamadas de entrada. Para encerrar as chamadas existentes, a [chamada de exclusão](../api/call-delete.md) deve ser usada em vez disso.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                |
| :-------------- | :--------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Não suportado                       |
| Delegado (conta pessoal da Microsoft) | Não suportado                       |
| Aplicativo     | Nenhum                                                       |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|motivos|String|O motivo da rejeição. Os valores possíveis `None`são `Busy` e`Forbidden` |
|callbackUri|String|Permite que os bots forneçam um URI de retorno de chamada específico, onde o resultado da ação de rejeição será lançado. Isso permite enviar o resultado para a mesma instância de bot específica que disparou a ação rejeitar. Se nenhum for fornecido, o URI de retorno de chamada global do bot será usado.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos
Os exemplos a seguir mostram como chamar essa API.

#### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp) 
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript) 
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)  
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="reject-an-incoming-call-with-none-reason"></a>Rejeitar uma chamada de entrada com o motivo ' nenhum '

##### <a name="notification---incoming"></a>Notificação-entrada

```http
POST https://bot.contoso.com/api/call
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "John",
              "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "ignored",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a>Notificação-excluído

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
